`Standards`**:** Are *documented agreements* containing `technical specifications` or other precise criteria that stipulate how a particular product or service should be *designed* or *performed*.

##### Common Standardization Organizations
- **Institute of Electrical and Electronics Engineers** `(IEEE)`**:** An *international society* composed of *engineering professionals*.
	- Best known for the *standardization* of `LAN technologies`. 
	- `Project 802`**:** aided in the standardization of Ethernet **(802.3)**
	- `Token Ring`**:** **(802.5)**
	- `Wireless LAN`**:** **(802.11)**

- **American National Standards Institute** `(ANSI)`**:** An organization composed of more than *one thousand representatives* from industry and government who work together to determine standards for `electronics`, `industry` and `other fields` such as `chemical and nuclear engineering`, `health and safety`, and `construction`.
	- Known for published standards such as **American Standard for Code Information Interchange** `(ASCII)` and **Small Computer System Interface** `(SCSI)`.

- **Electronic Industries Alliance** `(EIA)`**:** A *trade organization* composed of *representatives from electronics manufacturing firms* across the United States.
	- This organization writes `ANSI` standards and legislation favorable to the growth of computer and electronic industries.
 - **Telecommunications Industry Association** `(TIA)`**:** Focuses on *standards for IT, wireless satellite, fiber optics,* and *telephone equipment*.

- **Internet Engineering Task Force** `(IETF)`**:** An organization that is *responsible* for the `overall development` of the *internet* and the standardization of *internet-working technologies*.
	- Sets *standards* for how *systems* `communicate` over the *Internet*.
		- `Internet Society` **(ISOC)**`:` This *oversees* the overall *development of the internet*
		- `Internet Engineering Steering Group` **IESG**`:` This *oversees* the activities of `IETF` and *manages the process* used to introduce or update internet standards.
		- `Internet Architecture Board` **(IAB)**`:` This serves as the *technology advisory group of the* `internet Society` and is *responsible for the overall development of the protocols and architecture* associated with the `internet`**.**
		- `Internet Assigned Numbers Authority` **(IANA)**`:` This *oversees* internet `naming` and `addressing`; they are in *charge of all* `"unique parameters"` on the internet including `IP` addresses.

- **Organization For Standardization** `(ISO)`**:** The *International Organization for Standardization* `ISO` is an international standards organization responsible for a *wide range of standards*, including many that are relevant to networking.

##### Application Layer Protocols
- Provides *interfaces* for *application software* so that *applications can use network services*. The application layer protocol *designates transport layer protocols* and *ports*.
###### ----------------------------------
- `Simple Mail Transfer Protocol` **(SMTP)** - Refers to a *TCP/IP* protocol that *specifies a reliable and efficient transfer* of *electronic mail service* on the `internet`.
- `Post Office Protocol, Version 3` **(POP3)** - Refers to a *TCP/IP* protocol that is designed to allow a `workstation` to *retrieve mail* that the server is *holding for it*.
- `File Transfer Protocol` **(FTP)** - Refers to a *TCP/IP* protocol that enables the *sharing of computer programs* and/or *data* between hosts over a *TCP/IP* network. It uses `TCP` to *create a virtual connection* for *control information* and then *creates a separate* `TCP` *connection for data transfer*.
- `Network File System` **(NFS)** - Refers to a *TCP/IP* protocol that enables *computers* to *mount drives* on *remote hosts* and *operate them* as if they were `local drives`.
- `Trivial File Transfer Protocol` **(TFTP)** - A *small* and *simple alternative to* `FTP`  that uses `UDP` to *transfer files* between `systems`.
- `Domain Name Systems` **(DNS)** - Refers to a *TCP/IP* protocol that is *used on the internet for translating names of domains* and their p*ublicly advertised network nodes* into `IP Addresses`.
- `Simple Network Management Protocol` **(SNMP)** - Refers to a *TCP/IP* protocol that *monitors* and *controls the exchange of management information* between `networks` and `network components`; *it enables network administrators* to *manage configurations*, *statistics collection*, *network performance*, and *security*. `Three components`**:**
	- `Managed Devices`**:** *Collect* and *store* `management information` and make this information available to `NMSs` using `SNMP`.
	- `Agent`**:** Has *local knowledge* of `management information` and translates that information into a *form compatible* with `SNMP`.
	- `NMS`**:** *Executes applications* that *monitor* and *control* `managed devices`. `NMSs` provide the bulk of the *processing* and *memory resources required* for *network management*.
- `Terminal emulation Protocol Network` **(Telnet)** - Refers to a *TCP/IP* protocol that uses the `TCP` as the *transport protocol to establish a connection* between `server` and `client`.
	- Uses a *special software* called `daemon`, which is referred to as `remote host`
	- A connection using **Telnet** is called a `Virtual Terminal (VTY) session, or connection`.
- `Remote Login Application` **(rlogin)** - A `UNIX` *command* that allows *authorized users* to *log in* to other `UNIX` *machines* `(hosts)` on a network and to interact as if the user were physically at the host computer.
	- Once the user is *logged into the host*, the user can do *ANYTHING* that the host has permitted, such as *read, edit, or delete files.*
- `Hypertext Transfer Protocol` **(HTTP)** - Refers to an *application-level* protocol service and an internet standard developed by the `IETF` that supports the *exchange of information* on the `World Wide Web`, as well as on internal networks.
- `Hypertext Transfer Protocol over Secure Socket Layer` **(HTTPS)** - A *secure messages-oriented* communications protocol designed for use in conjunction with `HTTP`.
	- `Secure Sockets Layer` **(SSL)** - A *security protocol* that works at a *socket level*. This layer exists between the `TCP` layer and the *application layer* to *encrypt/decode* data and `authenticate` concerned entities.

##### TCP and UDP Connections
- Computers *running on the internet* communicate to each other using either the `Transmission Control Protocol` **(TCP)** or the `User Datagram Protocol` **UDP**.
	- `Transport Control Protocol` **(TCP)** - Refers to a `connection-oriented` *TCP/IP* standard transport layer protocol that provides *reliable data delivery*, *duplicate data suppression*, *congestion control*, and *flow control* on which many application protocol depend.
	- `User Datagram Protocol` **(UDP)** - Refers to a `connectionless` *TCP/IP* standard transport layer protocol that provides *unreliable*, *best-effort* service.
		- `UDP` is a *protocol* that sends *independent packets of data*, called `datagrams`, from *one computer* to *another* with *no guarantees about arrival*.
		- Sending `datagrams` is much like *sending a letter through the postal service*: The order of *delivery is not important* and is *not guaranteed*, and *each message is independent of any other*.

##### Port Numbers
- Data transmitted over the internet is accompanied by *addressing information* that *identifies the computer* and *the port for which it is destined*.
	- The computer is *identified* by its `32-bit IP Address`, which it uses `IP` to *deliver data* to the *specific computer* on the network.
	- `Ports` are *identified* by `a 16-bit number`, which `TCP` and `UDP` use to *deliver the data* to the *specific application*.
	- `Port Numbers` range from `0 to 65,535` because *ports* are represented by `16-bit numbers`.
	- The `port numbers` ranging from `0 - 1023` are *restricted*; they are reserved for use by *well-known services* such as `HTTP` and `FTP` and other *system services* called `well-known ports`.

| `Ports` | `Protocol`                        |
| ------- | --------------------------------- |
| **21**  | **File Transfer Protocol**        |
| **23**  | **Telnet Protocol**               |
| **25**  | **Simple Mail Transfer Protocol** |
| **80**  | **HyperText Transfer Protocol**   |
###### TCP and UDP Formats
`TCP Header Fields`
- `Source Port`**:** *Identifies the application* that *sends the segment*. This field is `16 bits long`.
- `Destination Port`**:** *Identifies the application* that *receives the segment*. This field is `16 bits long`.
- `Akcnowledgement Number`**:** *Indicates* the `sequence number` of the *next segment's first byte* that the `receiver` is expecting to receive.
	- The `value` of this field is `1 plus` the `sequence number of the last byte` in the *previous segment* that is successfully received.
	- This field is `32 bits long`.
- `Header length`**:** *Indicates the length* of the `TCP Header`.
	- The `unit` is `32 bits` **(4 bytes)**.
	- If there's no option content, the `value` of this field is `5`, indicating that the *header* contains `20 bytes`.
- `Reserved`**:** This field is *always set* to `0` as it is intended for *future protocol changes*.
	- It is `6 bits long`.
- `Control Bits`**:** Include `FIN`, `ACK`, and `SYN` *flags* which indicate the `TCP` **data segments** in different states.
- `Window`**:** Used for `TCP` *flow control*.
	- The `value` is the *maximum number of bytes* that are allowed by the `receiver`.
- `Checksum`**:** A *mandatory field* in which it is *calculated* and *stored* by the `sender` and *verified* by the `receiver`.

`UDP Header Fields`
- `Source Port`**:** *Identifies the application* that *sends the segment*. This field is `16 bits long`.
- `Destination Port`**:** *Identifies the application* that *receives the segment*. This field is `16 bits long`.
- `Length`**:** *Specifies* the `total length` of the `UDP header and data`.
	- The *possible minimum length* is `8 bytes` because the `UDP` header already *occupies* `8 bytes`.
- `Checksum`**:** **Field** refers to the `checksum` of the `UDP` **header** and `UDP` **data**.
	- This *field* is `16 bits long`.

##### SYN-ACK Handshake
- `Three-way handshake` - is a *method*, in which the `sender` and the `receiver` *inform* their respective *operating systems* that a *connection will be initiated* `before` the *actual data communication begins*.
	- `SYN` **->** *Synchronize*
	- `ACK` **->** *Acknowledge*
	- `FIN` **->** *Finish*

- `Sequence Number` **and** `Acknowledgement Number` - **Fields** to *implement reliable* and *ordered data transmission*.
- `Window Sliding Mechanism` - *Requires* the `sender` to *receive* an `acknowledgement` from the `receiver` *after transmitting* a certain *amount of data*.
- `TCP Shutdown` **(Four Way Handshake)** - Is engaged when the *data transmission* is *complete* in order to `disconnect` the `TCP` *connection* and *release system resources*.