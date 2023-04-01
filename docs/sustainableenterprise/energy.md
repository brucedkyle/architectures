# Energy cost containment


## Use cases

## Background

Most companies are committed to actions that make your operations more sustainable. At this point, some companies have set and published specific targets.

Businesses are seeking to balance the long-term imperative to protect the planet with the short-term need to preserve the bottom line. 

## Business problem

### Challenges / Business Drivers 

### Responses

| Business Problem | Solution |
| - | - |

## Business outcomes

## Solution overview

## Logical diagrams

[![logical diagram](./media/sustainableenterprise-logical.svg)](./media/sustainableenterprise-logical.svg)

_Figure 3. The personas and technologies that provide a platform for some of the biggest potential breakthroughs in managing a sustainable enterprise._


## Architecture

[![energy solution diagram](./media/energy-sd.svg)](./media/energy-sd.svg)

Energy cost containment
1. Collect sensor and energy consumption (energy, refrigerators, HVAC) across the enterprise. Unusual data can be from a piece of equipment that no longer functions, a walk-in refrigerator door being left open, HVAC that is providing temps outside of nominal ranges
2. Sensors report to Intelligent Assets and Facilities Management software that provides alerts on abnormal behavior of data from sensors
3. Alerts are sent to Sustainability Control Tower that takes actions to remediate consumption
4. Business automation provides consistent ways of handling alerts, sending work orders to facility and asset management software
5. Facility management software provides work orders, tracks the completion 
6. Facility manager is updated on the work orders and successful completion of the remediation steps
7. Sustainability Manager reviews KPI, update energy consumption metrics, sets energy consumption goals

## Action Guide

From a high-level perspective, the **Action Guide** represents a future state for organizations considering a comprehensive commitment. The idea is to outline a set steps that can be prioritized to reach that future state by adding new functionality to your existing systems.

- Automation
- Sustainability
- Modernization

| | Actionable Step | Implementation details |
| - | - | - |
| Automation | Reduce manual data processing | Automate energy data collection between finance and facility management systems |
| Automation | Advance the quality of capital, facility and environmental projects | Integrate data from multiple systems to get enterprise-wide view to capture and evaluate occupancy to align usage with business requirements and objectives.  |
| Automation | Optimize real estate portfolios | Centralize and integrate critical information at an enterprise level, giving organizations the ability to make the most cost-effective decisions |
| Automation | Amp up AI to make workflows smarter |  |
| Sustainability| Create digital twin of your facility. | Mirror and monitor building systems and troubleshoot problems before wasting resources on unnecessary or inaccurate repairs. |
| Sustainability | Include sustainability data in decision making | Integrate sustainability metrics in supply chain, facility management, and data center operations. |
| Sustainability | Decrease energy costs | Consolidate and measure energy cost reporting and provide systems to manage cost savings |
| Sustainability | Increase Green IT in your data center | Identify and measure application needs, shut down servers when they are not needed |
| Modernization | Modernization for modern infrastructures, scale hybrid cloud platforms | The decision for a future, Kubernetes-based enterprise platform is defining the standards for development, deployment and operations tools and processes for years to come and thus represents a foundational decision point. |
| Modernization | Modernize application deployment and operations practices | Include DevOps best practices to deploy, monitor, and maintain applications |

For specific steps on this approach, see **The Action Guide** details in [_Own Your Impact: Practical Pathways to Transformational Sustainability_](https://www.ibm.com/downloads/cas/6NJEKDD8) survey of 3,000 CEOs worldwide, that reveals sustainability's emergence onto the mainstream corporate agenda.

## Technology

The following technologies offered by Red Hat and IBM can augment the solutions already in place in your organization.

### Core systems

[*Red Hat OpenShift*](https://www.redhat.com/en/technologies/cloud-computing/openshift) Kubernetes offering, the hybrid platform offering allow deployment across data centers, private and public clouds offering choices and flexible for hosting system and services. You can manage clusters and applications from a single console, with built-in security policies with [_Red Hat Advanced Cluster Management_](https://www.redhat.com/en/technologies/management/advanced-cluster-management) and [_Red Hat Advanced Cluster Security_](https://www.redhat.com/en/technologies/cloud-computing/openshift/advanced-cluster-security-kubernetes).

[*Red Hat Ansible Automation Platform*](https://www.redhat.com/en/technologies/management/ansible) operate, scale and delegate automate IT services, track changes an update inventory, prevent configuration drift and  integrated with ITSM.

[*Red Hat OpenShift DevOps*](https://www.redhat.com/en/getting-started-devops) represents an approach to culture, automation and platform design intended to deliver increased business value and responsiveness through rapid, high-quality service delivery. DevOps means linking legacy apps with newer cloud-native apps and infrastructure. A DevOps developer can link legacy apps with newer cloud-native apps and infrastructure.

### Integration services

[*Red Hat OpenShift API Management*](https://access.redhat.com/documentation/en-us/red_hat_openshift_api_management/1/guide/53dfb804-2038-4545-b917-2cb01a09ef98) is a managed API traffic control and program management service to secure, manage, and monitor APIs at every stage of the development lifecycle.

[*Red Hat Intgration*](https://www.redhat.com/en/products/integration) is a comprehensive set of integration and messaging technologies to connect applications and data across hybrid infrastructures. It is an agile, distributed, containerized, and API-centric solution. It provides service composition and orchestration, application connectivity and data transformation, real-time message streaming, change data capture, and API management.

[*IBM Business Automation*](https://www.ibm.com/business-automation) delivers intelligent automations quickly with low-code tooling, such as business processes automation, decisioning software, robotic process automation, process mining, workflow automation, business process mapping, Watson Orchestrate, content services, and document processing.

[*IBM Data Fabric*](https://www.ibm.com/data-fabric) empowers your teams and works across the ecosystem by connecyting data from disparate data sources in multicloud envrionments. In particular, [_Watson Knowledge Catalog_](https://www.ibm.com/cloud/watson-knowledge-catalog) provides you users with a catalog tool for intelligent, self-service discovery of data, models. [_Watson Query_](https://www.ibm.com/products/watson-query) provides data consumers with a universal query engine that executes distributed and virtualized queries across databases, data warehouses, data lakes, and streaming data without additional manual changes, data movement or replication. 

### Sustainable enterprise sub-system

[*Envizi*](https://www.ibm.com/products/envizi) simplifies the capture, consolidation, management, analysis and reporting of your environmental, social and governance (ESG) data.

[*IBM TRIRIGA*](https://www.ibm.com/products/tririga/sustainability) harnesses the power of data and AI to infuse sustainability into your real estate and facilities management operations.

[*IBM Maximo Application Suite (MAS)*](https://www.ibm.com/products/maximo/sustainability) Infuse sustainability into your asset management by harnessing the power of data and AI.

[*IBM Turbonomic*](https://www.ibm.com/products/turbonomic) monitors resource consumption of applications within the data center. It provides FinOps engineering teams the ability to ensure your applications are performing efficiently, allowing cloud and ITOps teams to cut cloud spend and multiply ROI.

[*Transparent Supply*](https://www.ibm.com/products/supply-chain-intelligence-suite/blockchain-transparent-supply) provides supply chain management with a robust traceability solution.

## References

- [IBM journey to more sustainable facilities: IBM as client zero](https://www.ibm.com/blogs/internet-of-things/ibm-journey-to-more-sustainable-facilities-ibm-as-client-zero/)
- IBM Institute for Business Value [Balancing sustainability and profitability](https://www.ibm.com/thought-leadership/institute-business-value/report/2022-sustainability-consumer-research)
- [What is sustainability in business?](https://www.ibm.com/topics/business-sustainability)
- IBM Institute for Business Value [Sustainability at a turning point](https://www.ibm.com/downloads/cas/WLJ7LVP4) 

## Contributors

- Iain Boyle, Chief Architect, Red Hat
- Mahesh Dodani, Principal Industry Engineer, IBM Technology
- Thalia Hooker, Senior Principal Specialist Solution Architect, Red Hat
- Lee Carbonell, Senior Solution Architect & Master Inventor, IBM
- Eric Singsaas, Account Technical Lead, IBM Technology
- Mike Lee, Principal AI Ops Technical Specialist, IBM
- Rajeev Shrivastava, Account Technical Lead, IBM
- Bruce Kyle, Sr Solution Architect, IBM Client Engineering

