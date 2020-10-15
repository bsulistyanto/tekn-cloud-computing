Data as a Service (DaaS)
Data as a service (DaaS) is a cloud strategy used to facilitate the accessibility of business-
critical data in a well-timed, protected and affordable manner. DaaS depends on the principle that
specified, useful data can be supplied to users on demand, irrespective of any organizational or
geographical separation between consumers and providers.
DaaS eliminates redundancy and reduces associated expenditures by accommodating vital
data in a single location, allowing data use and/or modification by multiple users via a single update
point. Initially used in Web mashups, the DaaS strategy is often used by commercial organizations.
Data is usually located in relational databases inside corporate data centers. Typical business
applications include customer relationship management (CRM), enterprise resource planning (ERP),
e-commerce and supply chain systems.
Data has become the enabling technology for many of the recent innovations. "More data trumps
smarter algorithms" has been the mantra behind this revolution in computing. Given the rate at which
the data is produced, there is need for scalable solutions to extract information out of them. Allowing
the data to be stored in the cloud and be accessed without geographical and scalability limitations will
remove many bottlenecks in bringing data-oriented innovations. Current cloud architecture solves the
issues of accessibility and scalability, but poses several new challenges such as automatic
management of the service, pricing the data, and security of the data. This talk will include several
techniques to address these challenges using automatic physical design, service-based pricing, and
cryptographic mechanisms. Data  Information  Knowledge  Intelligence.
Data provided as a service was at first primarily used in web mashups, but now is being
increasingly employed both commercially and, less commonly, within organizations .Traditionally, most
enterprises have used data stored in a self-contained repository, for which software was specifically
developed to access and present the data in a human-readable form. One result of this paradigm is
the bundling of both the data and the software needed to interpret it into a single package, sold as a
consumer product. As the number of bundled software/data packages proliferated and required
interaction among one another, another layer of interface was required. These interfaces, collectively
known as enterprise application integration (EAI), often tended to encourage vendor lock-in, as it is
generally easy to integrate applications that are built upon the same foundation technology
The DaaS approach delivers the following benefits :
 Agility: Because data is easily accessible, customers can take immediate action and do not
require in-depth understanding of actual data.
 Affordability: Providers can construct a foundation and outsource the presentation layer, which
helps build highly affordable user interfaces and allows more feasible presentation layer change
requests.
 Data quality: Data accessibility is controlled through data services, which improves data quality,
as there is a single update point.
DaaS pricing models are classified into two main categories :
 Volume based model with two approaches: Quantity-based pricing and pay-per-call (PPCall)
 Data type based model
Data as a service operates on the premise that data quality can occur in a centralized place,
cleansing and enriching data and offering it to different systems, applications, or users, irrespective of
where they were in the organization, or on the network.
DaaS undertakes to provide the following advantages:
 Agility – users can move quickly, due to the simplicity of data access, and not needing extensive
knowledge of the underlying data. Data structures and location-specific requirements can be
modified to meet user needs.
 Cost-effectiveness – providers can build the base with the data experts and outsource the
presentation layer, which makes for very cost-effective user interfaces and makes change
requests at the presentation layer much more feasible.
 Data quality – data access is controlled through data services, which tends to improve data
quality, as there is a single point for updates. Once those services are tested, only regression
testing is needed, if they remain unchanged for the next deployment.
Architecture and common characteristics :
 Most database services offer web-based consoles, which the end user can use to provision and
configure database instances.
 Database services consist of a database-manager component, which controls the underlying
database instances using a service API. The service API is exposed to the end user, and permits
users to perform maintenance and scaling operations on their database instances.
 Underlying software-stack stack typically includes the operating system, the database and third-
party software used to manage the database. The service provider is responsible for installing,
patching and updating the underlying software stack and ensuring the overall health and
performance of the database.
 Scalability features differ between vendors – some offer auto-scaling, others enable the user to
scale up using an API, but do not scale automatically.
 There is typically a commitment for a certain level of high availability (e.g. 99.9% or 99.99%). This
is achieved by replicating data and failing instances over to other database instances..
The design and development of typical systems utilize data management and relational databases
as their key building blocks. Advanced queries expressed in SQL work well with the strict relationships
that are imposed on information by relational databases. However, relational database technology
was not initially designed or developed for use over distributed systems. This issue has been
addressed with the addition of clustering enhancements to the relational databases, although some
basic tasks require complex and expensive protocols, such as with data synchronization.
Modern relational databases have shown poor performance on data-intensive systems, therefore,
the idea of NoSQL has been utilized within database management systems for cloud based
systems. Within NoSQL implemented storage, there are no requirements for fixed table schemas, and
the use of join operations is avoided. Data models relying on simplified relay algorithms have also
been employed in data-intensive cloud mapping applications unique to virtual frameworks.
