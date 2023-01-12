# Inventory Optimization - Loss and Waste Management

A key focus when dealing with loss and waste management in relation to inventory optimization is how to handle unplanned or unforseen situations causing an inventory item be considered damaged or spoiled. If the situation or problem is rectified withing a well defined time window, there is a possibility of salvaging the product. In some cases once the incident occurs, there is no possibility of salvage and the product is considered damaged. Typically these events are external factors forced upon the business and cannot always be planned or predicted. 

To demonstrate the importance of inventory optimisation for any business, we will focus on two main use cases of an unanticipated exception:

- **Environment Exceptions** such as power outages or temperature changes that creates potential spoilage 
- **Product contamination or recall** such as foreign objects or bacteria occuring earlier in the processing or supply chain

We will start by defining the business problem and the two main use cases: Environmental Exceptions and Product contamination or recall, describe the challenges and business drivers organizations face. Next, we will provide an action guide, provide an overview of the solution, show a schematic of the two use cases: Environmental Exceptions and Product contamination or recall, and conclude with the technology used in the solution.

For a comprehensive inventory solution overview, see [Inventory Optimisation](inventory.md).


## Business problem

Loss and waste management is principally focused on ensuring food and food related products remain fit for consumption at the time they are sold to the end consumer. However, external factors outside the control of the business can cause food items to be marked as spoiled or damaged. The problem faced by the business is ensuring the overall loss and wastage is minimised.

*@ TODO: maybe add some temperature ranges here*

To prevent spoilage, food products must typically be stored and transported at temperatures within well defined ranges. For example:
- Frrozen food must be kept below a specific temperature at all times. If the temperature rises and food defrosts, it cannot be refrozen.
- Chilled food must be kept within a tenmperature range. The tenmperature can sometimes go above the higher limit for a short space of time before returning to the correct temperature, without becoming spoiled. If the high temperature is exceeded for a specified duration it must be considered spoiled.
- Ambient food does not require chilling, but needs to be stored withing a temperature range to ensure the product shelf life is maintained.

To keep food at the correct temperature, refrigeration and chilling during transport and storage are the primary options. Power outages will happen. The ability to deal with the situation within well defined time periods is critical to ensuring the loss and wastage is minimised. If the problem can be rectified quickly and easily, there is every chance the product can remain in perfect conditiona and be sold to a consumer. Failure to act quickly will result in spoilage and loss of the product.

Between farm and end consumer, food products generally go through multiple stages which vary depending on the end product. For convenience foods, there can be several manufuacturing steps, for fresh produce packaging and transport are the main stages. At any stage in the process, there is a possibility of contamination through foreign objects or bacteria. Both of which can trigger a recall of the food products. With any kind of contamination, a fast and efficient recall process to prevent the products beng purchased by consumers is vital.

All retailers handing and selling food products need processes to reduce food waste through external factors and ensure recall procedures in the event of contamination are fast, efficient and minimise any risk to public health.


## Use cases
The main use cases represented by loss management are:
- **Environmental Exceptions** such as power outage creates potential spoilage or Natural disaster  *@TODO: define*
- **Product contamination or recall** *@TODO: define*


## Challenges / Business Drivers 

**Challenges**

- *TODO: Add Challenge #1*
- *TODO: Add Challenge #2...*

**Drivers**

- *TODO: Add Driver #1*
- *TODO: Add Driver #2*


### Responses

All businesses that require a supply chain have unanticipated issues. 

| Business problem | Solution |
| - | - |
| Manual processes, limited capabilities of inventory management tools, and global operations pose a challenge for enterprises to manage and act on inventory and mitigate disruptions to meet actual demand. | Monitor and manage network inventory availability and anticipate actions due to unanticipated exception with alerts and recommended actions |
| Business process for handling unexpected issues may not be consistent across the enterprise | Gain detailed visibility into inventory characteristics at each location and provide transparency to inventory. Enable actionable inventory shifts across the enterprise |
| Visibility into actions needed and alternatives to anticipate and respond to inventory in an unanticipated event. | Provide actionable tasks, work orders, visibility for workers and supply chain partners to remove recalled items. Proactively replace items in response to demand.


## Action Guide

This use case implements actionable steps for *Automation* and *Modernization* in our Action Guide:
| Actionable Step | Implementation details |
| - | - |
| Create a world-class sensing and risk-monitoring operation | *TODO* |
| Accelerate automation in extended workflows | Business automation provides a systematic way to notifications, documentation of notifications, and creation of work orders. |
| Amp up AI to make workflows smarter | For Damaged or potential issues products, Control Tower monitors inventory connections to multiple core application systems foster visibility, create items in the work queue when revenue is at risk. When drilling down on the item, users can see where they have available inventory and receive recommendations about how much inventory can and should be ordered for replacement based on demand. |
| Modernization for modern infrastructures, scale hybrid cloud platforms | *TODO: Red Hat OpenShift...* |


## Solution overview

*TODO: Add business drivers paragraph and need to update diagram below with Loss and Waste Management-specific business drivers*

![solution diagram](./media/overview.png)

The solution uses the following technologies, which can be grouped into three main categories as shown in the following diagram:

- Core application systems. Often customer-provided technologies, such as order management, facilities management. These systems can be stand-alone applications, on premises and cloud services, databases. 
- Foundational infrastructure. The Red Hat/IBM solution is built on RedHat OpenShift. Data is routed through API management. Events are routed through Business Automation tools such as Business Automation Workshop. 
- Inventory Optimisation platform


## Solution principles

**True end-to-end visibility**. Remove data silos and create a unified view across supply chain data with a standard data platform. Personalized dashboards and insights provide a 360-degreee view of KPIs and significant events.

**Manage by exception**. Detect, display, and prioritize work tasks in real time. This allows clients to sense and react to issues quickly while managing risks and disruptions in a supply chain proactively.

**Intelligent workflows**. Actionable workflows can be customized to meet unique requirements and process steps required to automate actions within source transactional systems. Make informed decisions with a supply chain virtual assistant that provides responses to issues based on a client’s supply chain data using natural language search.

## Environment Exception

The following diagram shows the schematic for the understock use case.

![environmental exception schematic](./media/foodlossenvironmentexception.svg)

Food Loss - Environmental Exception steps:

<ol>
<li>Environmental event detected (e.g. Temperature out of range or loss of power)
<li>Notification sent to Risk Management module
<li>Inventory Control Tower processes risk and determines that it needs remediation
<li>Inventory Controller notified and determines inspection of facility and inventory is needed
<li>Remediation
<ol type="a"><li>Facilities personel performs remediation
<li>Inventory analyzed and remediated 
</ol>
</ol>

## Contamination/Recall 

The following diagram shows the schematic for the contamination recall use case.

Food Loss - Contamination recall steps:

![recall schematic](./media/recallschematic.svg)

<ol><li>External notification of food safety event
<li>Determine if supplier is affected
<li>Determine if locations received affected product
<li>Inventory Control Tower processes event data and creates remedediation action
<li>Colleague remediates inventory and counts, then removes product from inventory
<li>Location submits remediation data back to backend system for store credit
</ol>

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