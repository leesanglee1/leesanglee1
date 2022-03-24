# Data Virtualization
## Summary
### Issue
#### Data virtualization technology can be used to create virtualized and integrated views of data in memory (rather than executing data movement and physically storing integrated views in a target data structure), and provides a layer of abstraction above the physical implementation of data. (Gartner 2016)

#### Industry Use Cases:
  ##### BI and Big Data 
    Single view of entity
    Real time analytics and reporting
    Performance dashboards
    Virtual Data Marts
  ##### Operational
    Real-time operational views - Ex. summary of incidents, ranking, matrix of incident assignment, project status etc.
    Self-Service portal integration
    Enable Agile Business Intelligence - Ex. Operational decision support such as inventory control, risk management
  ##### Data Hub
    Data Services - Information as Service (IaaS), Information Feeds, Logical data Abstraction, Virtual Data Layer, Virtual MDM
    Provide access to a larger variety of data, including video, email and json documents and other Big Data sources often stored in platforms such as Hadoop.
    Integrate with Cloud Applications, such as Salesforce.com and cloud data services, such as GCP, Azure, AWS.

### Decision
Vendors select for POC:
  Tibco: https://www.tibco.com/products/data-virtualization
    Tibco DV is selected for POC.
  IBM: https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=overview
    IBM “Cloud Pak for Data” is selected for POC.
  Denodo: https://www.denodo.com/en/data-virtualization/overview 
    Denodo platform supports all the features but is too costly on per core basis compare to Tibco/IBM.
  Red Hat: 
    Acquired by IBM, so keeping IBM as only vendor.
  Oracle: 
    Their solution is primarily for their own platform and brings data from different data sources.
  Atscale: https://www.atscale.com/solutions/ 
    Supports data virtualization for only sql based data sources to create OLAP cubes.
  Data Virtuality: https://datavirtuality.com/en/ 
    Preferred way for data virtualization is through materializing entire data set in cache. Single server deployment not supporting clustering as of       now. 
  Actifio: https://www.actifio.com/platform/ 
    Supports virtualization through data cloning instead of data federation.
  Presto: https://prestodb.io/ 
    Open source sql engine for big data with ability to connect to various data sources. Not a data virtualization platform and misses key features like caching.
  Google: https://cloud.google.com/bigquery 
    Bigquery Supports integration with various data sources, but it is not data virtualization platform.


### Status
Assess: TIBCO was selected

Indicate how open you are to reviewing new options in this space going forward.

## Details
### Requirements
Major criteria used for evaluation
  Support for cloud and on-premise
  Data Source connectors supported out of box
  Methods supported to access data from platform
  Governance and security capabilities
  Development and runtime capabilities
  Metadata management and integration with external tools
  
### Considered Solutions
A list of possible Data Virtualization vendors were evaluated on paper and assessed for key requirements. TIBCO, IBM, and Denodo were selected for the actual POC activities.

### Rationale
Describe key reasons behind the decision, either for one option or against the others. Example: Bitwarden is open source and has a strong security track-record.
### Consequences
Describe any implications of the decision, and any drawbacks. Example: LastPass will be decommissioned in favor of BitWarden and we will need to provide a migration path.

## Related
Describe any knock-on decisions that arose as part of this assessment. Provide links to those decision documents wherever possible.
You may also consider documenting related requirements, artifacts, or principles here.

## Notes
Provide evaluation notes for each option that was evaluated: features, why it was considered, how it was evaluated and to what extent, conclusions.

To get user feedback on various solutions, we recommend the following polling framework:
Create a Google Form with scoring options 1-5: 
1. This would be a terrible mistake
2. This might work, but there are some issues to be addressed first
3. This is not my first choice, but I understand the appeal and would be willing to go along with a decision to use it
4. This is the best option from what we have available
5. This is the best solution ever

If someone provides a score of 2 or lower, ask them to document their specific concerns and see if they can be addressed. If they cannot be addressed, these must be captured in the Consequences section above. Find a solution where the majority of the participants rate it a 3 or higher.
