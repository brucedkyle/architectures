# Inventory Optimization - Loss Management

To demonstrate the importance of inventory optimisation for any business, this document will focus on main use cases of an unanticipated exception, such as:

- Power outage creates potential spoilage
- Natural disaster 
- Product recall
- Product contamination

For a comprehensive inventory solution overview, see [Inventory Optimisation](inventory.md).

## Business case

All businesses that require a supply chain have unanticipated issues. 

| Business problem | Solution |
| - | - |
| Manual processes, limited capabilities of inventory management tools, and global operations pose a challenge for enterprises to manage and act on inventory and mitigate disruptions to meet actual demand. | Monitor and manage network inventory availability and anticipate actions due to unanticipated acception with alerts and recommended actions |
| Business process for handling unexpected issues may not be consistent across the enterprise | Gain detailed visibility into inventory characteristics at each location – provide transparently to inventory. Enable actionable inventory shifts across the enterprise |
| Visibility into actions needed and alternatives to anticipate and respond to inventory in an unanticipated event. | Provide actionable tasks, work orders, visibility for workers and supply chain partners to remove recalled items. Proactively replace items in response to demand.

## Solution overview

The technologies can be grouped into three main categories as shown in the following diagram:

- Core application systems. Often customer-provided technologies, such as order management, facilities management. These systems can be stand-alone applications, on premises and cloud services, databases. 
- Foundational infrastructure. The Red Hat/IBM solution is built on RedHat OpenShift. Data is routed through API management. Events are routed through Business Automation tools such as Business Automation Workshop. 
- Inventory Optimisation platform

![solution diagram](./media/overview.png)

## Solution principles

**True end-to-end visibility**. Remove data silos and create a unified view across supply chain data with a standard data platform. Personalized dashboards and insights provide a 360-degreee view of KPIs and significant events.

**Manage by exception**. Detect, display, and prioritize work tasks in real time. This allows clients to sense and react to issues quickly while managing risks and disruptions in a supply chain proactively.

**Intelligent workflows**. Actionable workflows can be customized to meet unique requirements and process steps required to automate actions within source transactional systems. Make informed decisions with a supply chain virtual assistant that provides responses to issues based on a client’s supply chain data using natural language search.

## Environment Exception

The following diagram shows the workflow for the environment exception use case.

![environmental exception workflow](./media/environmentexceptionworkflow.png)

Food Loss - Environmental Exception steps:

<ol>
<li>Environmental event detected (e.g. Temp out of range, loss of power)
<li>Notification sent to Risk Management module
<li>Inv Ctrl Tower processes risk and determines that it needs remediation
<li>Inv Controller notified and determines inspection of facility and inventory is needed
<li>Remediation
<ol type="a"><li>Facilities personel performs remediation
<li>Inventory analyzed and remediated 
</ol>
</ol>

The following diagram shows the schematic for the understock use case.

![environmental exception schematic](./media/foodlossenvironmentexception.svg)

## Contamination/Recall 

The following diagram shows the workflow for the contamination recall use case.

![contaimination recall workflow](./media/contaminationrecallworkflow.png)

<ol><li>External notification of food safety event
<li>Determine if supplier is affected
<li>Determine if locations received affected product
<li>Inv Ctrl Tower processes event data and creates remedediation action
<li>Colleague remediates inventory and counts, then removes product from inventory
<li>Location submits remediation data back to backend system for store credit
</ol>

The following diagram shows the schematic for the contamination recall use case.

![recall schematic](./media/recallschematic.svg)

## Technology

The following technology was chosen for this solution:

*Red Hat OpenShift* Kubernetes offering, the hybrid platform offering allow deployment across data centers, private and public clouds as it brings choices and flexible for hosting system and services.

*Red Hat Ansible Automation Platform* operate, scale and delegate automate IT services, track changes an update inventory, prevent configuration drift and  integrated with ITSM.  

*Business Automation Workflow* automate business processes, case work, task automation with Robotic Process Automation (RPA) and Intelligent Automation such as conversation intelligence. 

*IBM Supply Chain Control Tower* provides actionable visibility to orchestrate your end-to-end supply chain network, identify and understand the impact of external events to predict disruptions, and take actions based on recommendations to mitigate the upstream and downstream effects.

*IBM Sterling Intelligent Promising* provides shoppers with greater certainty, choice and transparency across their buying journey. It includes:

- *IBM Sterling Fulfillment Optimizer with Watson* to determine the best location from which to fulfill an order, based on business rules, cost factors, and current inventory levels and placement
- *Sterling Inventory Visibility* to processes inventory supply and demand activity to provide accurate and real-time global visibility across selling channels.

| Use Case | The Problem | The Solution | The Benefits and Implications |
| - | - | - | - |
| Automated processes | Manual input and follow up | Business automation provides a systematic way to notifications, documentation of notifications, and creation of work orders. | Actions follow a consistent business process and can be easily updated as needs change | 
| Damaged or potential issues products | Facilities issues can immediately impact product liability, lead to lost revenue and decreased brand / retailer loyalty. | Control Tower monitors inventory connections to multiple core application systems foster visibility,  create items in the work queue when revenue is at risk. When drilling down on the item, users can see where they have available inventory and receive recommendations about how much inventory can and should be ordered for replacement based on demand. | Action can be taken directly from the Control Tower user interface. Product situations are efficiently managed and OOS are avoided with minimal human intervention. |
| API Management | Separation of systems, control and monitoring of access, providing consistent user authentication and security between platforms | API Manages the access and permissions required for data between systems. | Improved security, monitoring of frequency of access between systems |
| Supply intelligence, inventory analysis | Avoid discarding items not included in recall, contamination Provide alternative products that can be substituted. Determine alternative locations or steps to stage product | Supply intelligence and inventory analytics provides record of product details, visibility into substitute products, - visibility of item locations, suggested remediation steps | Supplies can be immediately removed from sale, substitute product offered, steps to ship unaffected products as needed based on actual demand |
| Colleage and partner engagement | Quick sharing data between enterprise silos and to partners who can provide solutions | Visibility into recall issues |

## Similar use cases

See:

- [Product timeliness](timeliness.md)
- [Demand risk](demandrisk.md)

For a comprehensive inventory solution overview, see [Inventory Optimisation](inventory.md).

## Downloads

View and download all of the **Inventory Optimisation diagrams** shown in previous sections in our open source tooling site.

- PowerPoint: [Open Workflow Diagrams](./downloads/InventoryOptimisation.pptx)
- DrawIO: [Open Schematic Diagrams](./downloads/InventoryOptimisation.drawio)

## Contributors

- Iain Boyle, Red Hat
- Bruce Kyle, IBM
- Mahesh Dodani, IBM
- Thalia Hooker, Red Hat
- Jeric Saez, IBM
- Mike Lee, IBM
- Lee Carbonell, IBM
- James Stewart, IBM