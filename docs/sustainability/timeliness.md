# Inventory Optimisation - Product Timeliness

Foods and ingredients expire or become unusable at some point. Manufactured parts and goods also experience decay and deterioriation. Each of these may be measured.

In the food industry, you may see different terms and date types on the packaging, the following are common practices and their meanings according to the USDA and FDA as explained in [Expiring Products – Food & Ingredients](https://www.canr.msu.edu/news/expiring-products-food-ingredients) by Michigan State University:

- Best if used by/before: this term is NOT an expiration date, rather it’s the date where the food may be at its best quality 
- Use by: on any food OTHER than infant formula, this term is NOT an expiration date, rather it’s the date where the food may be at its best quality. If “used by” is present on infant formula, it’s an expiration date, and you should discard the infant formula after the use by date.  
- Sell by: this term is NOT an expiration date, rather it’s the date where the food may be at its best quality 
- Freeze by: this term is NOT an expiration date, rather it’s the date where the food should be frozen to maintain the best quality 
- Expiration or EXP: this is an expiration date and usually only found on infant formula and some baby foods 
- Guaranteed fresh: this term is NOT an expiration date, rather it’s the date where the food may be at its best quality 
 
Other products, particularly pharmaceuticals, must be used within specific time frames to be warantted or to be considered safe and effective. 

Manufactured parts may be warranteed for specific periods or number of uses. For example, manufactured parts must be replaced when outside of certain tolerances.

Some products may still continue to be useful beyond their expiration date or use. 

For a comprehensive inventory solution overview, see [Inventory Optimisation](inventory.md).


## Business problem

Product liability claims can wreck a business. 

Defects and liability risks affect product manufacturers, designers, distributors, wholesalers, and retailers. Physical or digital items that omit adequate warnings, injure a third party, or cause a wrongful death can lead to lawsuits for any party involved in the product.

## Use Cases

How should a business track and respond to issues?

- Responding to _Shelf life_ defines a set of actions to be taken with products that expire on specific dates and must be removed from use or sale. For example, food can expire and need to be removed from shelves. 
- _Timeliness_ defines a set of actions that can be taken when products expire, but that may be still have some benefit. For example, seasonality of clothing can be warehoused until the following year.

In both shelf life and timeliness, you will want to plan and to take proactive steps in anticipation of product expirations.

## Challenges / Business Drivers 

**Challenges**

- Tracking items for shelf life and timeliness
- Taking actions, such as product removal, replacement, work order tracking to demonstrate the product is handled with due care

**Drivers**

- Public safety
- Product liability claims
- Demonstrating due diligence for safety


### Responses

Many goods offered in retail and supplier businesses expire. 

| Business problem | Solution |
| - | - |
| Manual processes, limited capabilities of inventory management tools, and global operations pose a challenge for enterprises to manage and act on inventory and mitigate disruptions to meet actual demand. | Monitor and manage network inventory availability and anticipate actions due to expiration of products with alerts and recommended actions. |
| The lack of pertinent product information (remaining shelf life, ambient temperature, etc.) and poor data flow across partners lead to inefficient inventory management, wastage and lost sales. | Gain detailed visibility into inventory characteristics at each location – e.g., by remaining shelf life, time-since-harvested. Maintain freshness by acting on alerts received when items are at risk. |
| Visibility into actions needed and alternatives to anticipate and respond to inventory as items approach end of shelf life. | Provide actionable tasks, work orders, visibility for workers and supply chain partners to remove end of life items. Proactively replace items in response to demand. |


## Solution overview

*TODO: Add business drivers paragraph and need to update diagram below with Product Timeliness-specific business drivers*

![solution diagram](./media/overview.png)

The solution uses the following technologies, which can be grouped into three main categories as shown in the following diagram:

- Core application systems. Often customer-provided technologies, such as order management, facilities management. These systems can be stand-alone applications, on premises and cloud services, databases. 
- Foundational infrastructure. The Red Hat/IBM solution is built on RedHat OpenShift. Data is routed through API management. Events are routed through Business Automation tools such as Business Automation Workshop. 
- Inventory Optimisation platform


## Solution Principles

**True end-to-end visibility**. Remove data silos and create a unified view across supply chain data with a standard data platform. Personalized dashboards and insights provide a 360-degreee view of KPIs and significant events.

**Manage by exception**. Detect, display, and prioritize work tasks in real time. This allows clients to sense and react to issues quickly while managing risks and disruptions in a supply chain proactively.

**Intelligent workflows**. Actionable workflows can be customized to meet unique requirements and process steps required to automate actions within source transactional systems. Make informed decisions with a supply chain virtual assistant that provides responses to issues based on a client’s supply chain data using natural language search.

## Timeliness/Shelf life

The following diagram shows the schematic for the Timeliness/Shelf life use case.

![shelf life schematic](./media/shelflifechematic.svg)

Timeliness/Shelf life steps:

1. Inventory Control Tower hueristics determines product inventory is near its "Use by" date
2. Inspects current inventory
3. Notifies the Inventory Controller to take action
4. Creates replenishment order
5. Engages partners (Charity, recycler) to remediate expired or near expired stock


## Action Guide

This use case implements actionable steps for *Automation* and *Modernization* in our Action Guide:
| Actionable Step | Implementation details |
| - | - |
| Create a world-class sensing and risk-monitoring operation | *TODO* |
| Accelerate automation in extended workflows | Business automation provides a systematic way to notifications, documentation of notifications, and creation of work orders. |
| Amp up AI to make workflows smarter | For expiring products, Control Tower monitors inventory levels at all locations in a client’s network and creates items in the work queue when revenue is at risk. When drilling down on the item, users can see where they have available inventory and receive recommendations about how much inventory can and should be ordered for replacement based on demand. |
| Modernization for modern infrastructures, scale hybrid cloud platforms | The decision for a future, Kubernetes-based enterprise platform is defining the standards for development, deployment and operations tools and processes for years to come and thus represents a foundational decision point.  |


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
| Expiring products | Expiring item situations lead to lost revenue and decreased brand / retailer loyalty. | Control Tower monitors inventory levels at all locations in a client’s network and creates items in the work queue when revenue is at risk. When drilling down on the item, users can see where they have available inventory and receive recommendations about how much inventory can and should be ordered for replacement based on demand. |  Action can be taken directly from the Control Tower user interface. Expiring product situations are efficiently managed and OOS are avoided with minimal human intervention. |
| API Management | Separation of systems, control and monitoring of access, providing consistent user authentication and security between platforms. | API Manages the access and permissions required for data between systems. | Improved security, monitoring of frequency of access between systems. Improved system maintainability. |

## Similar use cases

See:

- [Demand risk](demandrisk.md)
- [Product timeliness](timeliness.md)

For a comprehensive inventory solution overview, see [Inventory Optimisation](inventory.md).

## Downloads

View and download all of the **Inventory Optimisation diagrams** shown in previous sections in our open source tooling site.

- PowerPoint: [Open Workflow Diagrams](./downloads/InventoryOptimisation.pptx)
- DrawIO: [Open Schematic Diagrams](./downloads/InventoryOptimisation.drawio)

## Contributors

- Iain Boyle, Red Hat
- James Stewart, IBM
- Bruce Kyle, IBM
- Mahesh Dodani, IBM
- Thalia Hooker, Red Hat
- Jeric Saez, IBM
- Mike Lee, IBM
- Lee Carbonell, IBM