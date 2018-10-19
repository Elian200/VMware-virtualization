
# Introduction to the Private Cloud


# Objectives

- Describe the architecture of a private cloud
- Identify the hardware requirements for a private
    cloud.
- Describe the software requirements for a private
    cloud.
- Describe uses for a private cloud.


# Making the Transition to Cloud Computing

- In the past:
    - Application software had to be installed on a
       user’s computer.
          - A license for each application had to be
             purchased.
- Client/server model
    - Server computers with enhanced capabilities
       and large storage devices are used to store
       data for multiple users.
    - Require the purchase of multi-user licenses.


# Client/Server Model
![Downloads](https://www.tutorialspoint.com/data_communication_computer_network/images/client_server.jpg)
 
- Cloud computing
    - Provides applications from a server that are
       executed and managed by a client’s Web
       browser.
    - Cloud server providers have complete control
       over applications.
          - Eliminates the need for version upgrades or
             license management on client computers.
- Software as a Service (SaaS)
    - Term used to describe the application programs
       offered through cloud computing.

- Any “Web-friendly” device connected to the
    Internet can access the same pool of computing
    power and files in a cloud computing environment.

- A Web site or Web application that is hosted in a
    public cloud.
       - Has additional processing power available
          within the cloud.
             - If a Web site becomes more popular, the
                cloud automatically directs more computers
                to serve pages.
             - If site loses popularity, the cloud will scale
                down number of servers to reduce cost of
                service.
- Cloud computer is popular for its “pay-as-you-go”
    pricing model.


- A private cloud offers same features and benefits
    as public clouds.
       - Offers more control over enterprise and
          customer data, security, and regulatory
          compliance.


# Server Virtualization

- Virtualization: use of software to simulate a
    physical computing environment
       - And the use of virtual hardware on which you
          can install a number of operating systems
          (OSs) and interact with them
- Hypervisor: allows multiple operating systems
    (called guests) to run concurrently on a host
    computer
       - Presents a virtual operating platform to the
          guest operating systems and manages their
          execution


# Hypervisor Virtualization

# Technology


# Server Virtualization

- A standard hardware system environment is
    provided within each virtual machine for each
    guest OS
       - The OS and software within each virtual
          machine are unaware of the other virtual
          machines
- Virtualization permits installation of a new OS on
    an existing computer without disrupting the
    previous OS
- Server virtualization in cloud computing enables
    rapid provisioning
       - Addition of virtual machines to meet increased
          demands for processing online requests


# Storage Virtualization

- In a network, a file server is a computer that
    has the primary purpose of providing shared
    disk access
       - It is not intended to run applications for its
          clients


# Storage Virtualization

- Network-attached storage (NAS): file-level data
    storage on a computer network that provides data
    access to clients
       - NAS systems usually contain two or more hard
          drives that are combined and arranged in
          Redundant Array Independent Disk (RAID)
          arrays
- Multiple disk drives can work together to form a
    disk array
       - Data that is frequently needed is retrieved from
          a cache
- Redundant components such as RAID, processing
    modules, and power supplies increase availability


# NAS with RAID


# Disk Array


# Storage Virtualization

- Disk arrays can be consolidated into a storage area
    network (SAN)
       - Data appears to be stored to a single source
       - Easier than managing individual disks on
          multiple servers
- A SAN uses the principle of storage virtualization
    - Handles storage as a unified whole
    - Enables virtual machines to use data from a
       unified storage entity rather than individual
       disks
- Logical unit number (LUN): a unique identifier used
    to designate a unit of storage


# Storage Virtualization

- Thin provisioning: approach where LUNs for new
    servers can be created
       - More disk space can be assigned on those
          servers than the actual amount of space
          configured for the SAN
             - Example: server that hosts a database may
                appear to have 100 GB allocated for data
                storage when only a small percentage of
                that is actually allocated


# Storage Area Network


# Network Virtualization

- Virtual LAN (VLAN): group of PCs, servers, and
    switches that appear to be connected to a single,
    logical network segment
- In network virtualization:
    - A network’s resources and client/server system
       are combined and put on a virtual network
    - This network treats all hardware and software as
       a single collection of resources that can be
       accessed regardless of physical boundaries
    - Requires routers and switches to perform more
       services, such as access control, path isolation,
       and edge services


# Virtualized Networks


# Clustering

- Clustering: connecting multiple computers to make
    them work as a unified system
       - Increases a computer’s load balancing and
          redundancy
- Load balancing: distributes processing across
    multiple servers
       - Might allocate incoming requests evenly to all
          servers or it might send requests to the next
          available server


# Clustering

- Redundancy: ability of a cluster to respond
    gracefully to an unexpected hardware or software
    failure
       - Failover: capability to switch to a redundant or
          standby server automatically when the active
          server fails


# Clustered Computers


# Role-Based Security

- Role-based security: provides finer control over
    permissions in a virtualized environment
       - Groups of virtual machine instances determine
          which machines are available for particular user
          tasks
       - Administrators specify operations that a user can
          perform based on group membership
- Self-service user role
    - Members of this role can mange their virtual
       machines under certain controls
    - Role can also be used with a quota to limit the
       number of virtual machines available to a user


# Cloud Computing Services

- Infrastructure as a Service (IaaS) – service
    provider pays for servers, network equipment,
    storage, and backups
       - Customers pay only for the service
- Platform as a Service (Paas) – service provider
    offers business solutions for users
- Software as a Service (SaaS) – customers pay to
    use the service provider’s software
       - Example: Google Apps


# Hardware Diagram for

# Private Cloud


# Active Directory Domain

# Services

- AD DS provides a distributed database that
    stores and manages information about network
    resources
       - Uses a hierarchical structure
       - Structure includes the:
          - Active Directory forest
          - Domains in the forest
          - Organizational units (OUs) in each domain
- A server that runs AD DS is called a domain
    controller


# Active Directory Domain

# Services

- Security is integrated with AD DS through:
    - Logon authentication
       - Uses a single network logon to manage the
          AD DS directory data throughout the
          network
       - Authorized users can also use a single
          network logon to access resources anywhere
          in the network
    - Access control to resources
       - Policy-based administration centralizes the
          management of computers
       - Group Policy defines the settings and
          allowed actions for users and computers


# Domain Name Service

- DNS server role:
    - Provides a name resolution process that
       enables users to locate network computers by
       querying for a user-friendly name instead of
       an IP address
    - Queries can include requests such as:
       - Names of Web sites
       - Network computers
       - Computers on the Internet


# Hyper-V Hypervisor

- Windows Server 2008 R2 hypervisor
    - Enables the creation of a virtualized server
       computing environment
    - Use Hyper-V to manage virtual machines and
       their resources
- Hyper-V role consists of several components:
    - Hypervisor
    - Parent and child partitions
    - Virtual machines and guest operating systems
    - Synthetic and emulated devices
    - Integration services


# Hyper-V Hypervisor

- Hyper-V hypervisor: core component of Hyper-V
    - Responsible for creating and managing isolated
       execution environments called partitions
    - Sits directly on hardware and controls access
       from partitions to physical processors


# Hyper-V Hypervisor

- When Hyper-V hypervisor loads for the first time
    it creates a parent partition (first virtual machine)
- Importance of parent partition:
    - Controls all hardware devices and is
       responsible for allocating physical memory to
       the partitions
    - Directs the hypervisor to create and delete
       child partitions
          - Child partitions do not have access to
             physical hardware
          - I/O requests are routed through the parent
             partition


# Hyper-V Hypervisor

- Operating systems installed within child partitions
    are referred to as guest operating systems
- Virtual devices exposed to guest operating
    systems fall into one of two broad categories:
       - Emulated virtual devices – software
          implementation of a typical PCI device (appears
          as a physical PCI device)
       - Synthetic virtual devices – only function with
          Hyper-V and are also implemented in software
- Using synthetic devices creates less processor
    overhead than using emulated devices


# Hyper-V Hypervisor

- Communication mechanism between partitions:
    - Virtualization Service Provider (VSP) – runs in
       the parent partition and directly communicates
       with hardware drivers
    - Virtualization Service Client (VSC) – runs in the
       child partitions and presents the virtual device to
       each child partition
          - Each VSC has a corresponding VSP in the
             parent partition
    - VMBus – point-to-point memory bus is used for
       communication between VSP and VSC


# Hyper-V Hypervisor

- Enlightenments – Microsoft term given to
    implementations in virtual environments that
    reduce overhead and improve guest operating
    system performance
- Integration Services for Hyper-V – provided by
    Microsoft and available for all supported guest
    operating systems
       - Meant to provide better integration between
          child and parent partitions
       - Provide enhancements such as mouse
          integration, time synchronization, and the ability
          to shut down the guest operating system from
          the management console


# Hyper-V Hypervisor

- Hyper-V Manager – management console for
    Hyper-V
       - Divided into three panes
          - Surveyor – used to select the host server
          - Information – provides information about the
             host computer
          - Actions – shows the available actions for the
             host computer and selected virtual machine
                - Top half lists actions available for host
                   computer
                - Bottom half lists actions available for the
                   selected virtual machine
- New Virtual Machine Wizard – simple and flexible
    way to create a virtual machine


# Hyper-V Manager


# Summary

- Cloud computing is the use of multiple server
    computers on a digital network that work together
    as if they were one computer
- Virtualization uses software to simulate a physical
    computing environment on which you can install a
    number of OSs and interact with them
- Virtualization requires specific hardware for the
    host computers to function properly
- The amount of memory required for effective
    processing is determined by the number of virtual
    machines that will run concurrently


# Summary

- The number of network adapters needed is
    determined by the minimum number of networks
    required for the creation of private clouds
- The Internet Small Computer System Interface
    (iSCSI) is an IP-based storage networking
    standard for linking host computers to data
    storage facilities


