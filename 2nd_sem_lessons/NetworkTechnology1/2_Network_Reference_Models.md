- `Network Topologies` **-** It is a *schematic description* of a *network arrangement*, *connecting various nodes* `(sender and receiver)` through lines of *connection*.

##### Different Topologies
- `Star Topology` **-** Computers are connected to a *single hub* through a *cable*. This *hub* is the *central node* while all other nodes are *connected to it*.
	- **Advantages:**
		- `New nodes can be easily added to the network`
		- `Communication data must be forwarded by the central node, which facilitates network monitoring`
	- **Disadvantages:**
		- `Faults on the central node affect the entire network's communication`

		
- `Bus Topology` **-** Every computer and network device is connected to a *single cable*. When it has exactly *two* `2` *endpoints*, then it is called `Linear Bus Topology`. All *nodes* are connected through a bus. `(EX: Coaxial Cable)`
	- **Advantages:**
		- `Installation is simple and cable resources are saved`
		- `Generally, the failure of a node does not affect the communication of the entire network`
	- **Disadvantages:**
		- `A bus fault affects the communication of the entire network`
		- `The information sent by a node can be received by all other nodes, resulting in low security`

		
- `Ring Topology` **-** Forms a *ring* as each computer is *connected to another computer*, with the last *one* `1` connected to the *first --* exactly *two* `2` neighbors for each device.
	- **Advantages:**
		- `Cable resources are saved`
	- **Disadvantages:**
		- `Difficult to add nodes`
		- `Original ring must be interrupted before new nodes are inserted to form a new ring`


	
- `Tree Topology` **-** Has a *root node* and all other nodes are *connected to it*, forming a *hierarchy*. Also called `Hierarchical Topology`. It should at least have *three* `3` *levels* to the hierarchy.
	- **Advantages:**
		- `Multiple star networks can be quickly combined`
		- `Facilitating network expansion`
	- **Disadvantages:**
		- `A fault on a node at a higher layer is more severe`




- `Mesh Topology` **-** A *point-to-point connection* to other nodes or devices. All the network nodes are *connected.*
	- `Partial Mesh Topology` **-** Some system are *connected*, but some devices are only connected to *two* or *three* devices.
		- **Advantages:**
			- `The cost of a partial-mesh is lower than the full mesh`
		- **Disadvantages:**
			- `Reliability of a partial-mesh is lower than full mesh`
	- `Full Mesh Topology` **-** Each node or device is *connected*.
		- **Advantages:**
			- `High reliability and high communication efficiency`
		- **Disadvantages:**
			- `Each node requires a large number of physical ports and interconnection cables. As a result, the cost is high, and it is difficult to expand`
- `Hybrid Topology` **-** It consists of a *mix of two* `different types of topologies`, merging as one network.
	- In *actual networking*, multiple `types of topologies` may be combined based on the cost, communication efficiency, and reliability requirements.


##### Common Network Devices
- `Terminal Devices` - It is the *end-device* of the *data communication system.* It provides the necessary functions required by the `user access protocol operations.`
	- `Data Terminal Equipment` **(DTE)** - *Computers*, *Phone*, *handsets*, *printers*, and *servers*.
	- `Network Interface Card` **(NIC)** - Is a *key component* that connects *directly to a device* that allows access to a `network` such as an internet.

- `Switch` - It is the device *closest to end-users*, used to access the network and switch `data frames`.
	- Belongs at `access layer`, `layer 2`
	- `Ethernet Switches`
	- `Broadcast Domain`, a *set of nodes* that can receive broadcast packets from a node.
	- Can do the following:
		- `Data Frame Switching`
		- `Access to end-user devices`
		- `Basic access security functions`
		- `Layer 2 Link redundancy`

- `Router` - A *network layer* device that forwards *data packets* on the internet.
	- `Modem`, a device that connects a *network* to the *internet*. Takes signals from `ISP` and translates them into signals connected to the local devices.
	- `Gateway`, term for a router that provides *functions* such as *protocol conversion*, *route selection*, and *data exchange*.
 
 - `Firewall` - A *network security* device used to ensure *secure communication between two networks*.
 - `Wireless Devices` - Uses *radio waves*, *laser*, and *infrared signals* to replace some or all transmission media in a *wired LAN*.
 - Common Wi-Fi is a `WLAN technology` based on the *IEE 802.11 family* of standards.
	 - `Fat Access Point` **(Fat AP)** - Applies to homes. Works *independently* and needs to be configured separately. *Simple functions* and *low costs*.
	 - `Fit Access Point` **(Fat AP)** - Applies to *medium and large sized enterprises*. Needs to work with *AC* and managed and configured by the *AC*.
	 - `Access Controller` **AC** - Generally *deployed* at the *aggregation layer* of the entire network. Provides *wireless data control services* like `large capacity`, `high performance`, `high reliability`, etc.


##### Networking Based on Geographical Coverage
- `Local Area Network` **(LAN)** - Covers an area of a few square kilometers
- `Metropolitan Area` **(MAN)** - A *Large-sized LAN*, requiring high costs but can provide a higher transmission rate. Covers university campus or city.
- `Wide Area Network` **(WAN)** - Covers an area of *several kilometers or larger*. Connect several `LANs` or `MANs` that are far from each other.


##### OSI REFERENCE MODEL
- `Open Systems Interconnection model` - A *descriptive network scheme*. How information or  data makes its way from *application* programs through a network medium to another *application* *program located* on *another network*.
	- `LAYER 1` **Application Layer** - Closest to the user. Provides network services to the user's applications such as spreadsheet programs, word processing programs, and bank terminal programs.
	- `LAYER 2` **Presentation Layer** - *Ensures* that the information that the application layer of one system sends out is *readable by the application*.
	- `LAYER 3` **Session** - Defines how to *start*, *control* and *end conversation* between sessions.
	- `LAYER 4` **Transport** - *Regulates information* flow to ensure `end-to-end` connectivity between host applications reliably and accurately.
	- `LAYER 5` **Network** - *Defines* `end-to-end delivery` *of packets*. It defines how routing works and how routes are learned so that the packets can be delivered.
	- `LAYER 6` **Data Link** - *Provides access* to the networking media and physical transmission across the media and this enables that data to locate its *intended* *destination on the network*.
	- `LAYER 7` **Physical Layer** - Deals with the *physical characteristics* of the transmission medium.

##### TCP/IP Model
- `Networking Model` with a set of *communication protocols for the internet and similar networks*.
- `Internet Protocol` **IP** - Provides basic communication.
- `Transmission Control Protocol` **TCP** - Provides *key functions* that applications need.
	- `APPLICATION LAYER`**:** Represents an interface through a *variety of protocols* that enables services to be applied to *end-user* application processes.
	- `TRANSPORT LAYER`**:** Responsible for reliable *end-to-end data* delivery from the *source host* to the *destination host*.
	- `INTERNET LAYER`**:** Is responsible for the *delivery of service requests* that respond from the `transport layer` and have them arrive at their *destination* through the *"virtual network"* image of the internet.
	- `NETWORK ACCESS LAYER`**:** Also called the `host-to-network layer`, which is concerned with all of the issues that an *IP packet* requires to make a *physical link to the network media*.


`OSI MODEL` is a *logical and conceptual model* that defines network communication used by systems open to interconnection and communication to other systems.
- **Vertical** `Approach`
- **Connection** `Oriented`
- Developed by `ISO` **International Standard Organization**
- Helps you *standardize* `router`, `switch`, `motherboard`, and other hardware

`TCP/IP` helps you determine how a *specific computer* should be connected to the internet and how you can be *transmitted between* them.
- **Horizontal** `Approach`
- Both **Connection** `Oriented` and **Connectionless**
- Developed by `ARPANET` **Advanced Research Project Agency Network**
- Helps you *establish a connection* between `different types of computers`.