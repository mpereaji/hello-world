**Open Data Model (ODM)**
=========================
	
**Overview**
------------

This document describes a strategy for creating an open data model (ODM) for
Apache Spot (incubating) (formerly known as “Open Network Insight (ONI)”) in
support of cyber security analytic use cases. It also describes the use cases
for which Apache Spot (incubating) running on the Cloudera platform is uniquely
capable of addressing along with the data model.

**Apache Spot (incubating) Open Data Model Strategy**
-----------------------------------------------------

The Apache Spot (incubating) Open Data Model (ODM) strategy aims to extend
Apache Spot (incubating) capabilities to support a broader set of cyber security
18	use cases than initially supported. The primary use case initially supported by
19	Apache Spot (incubating) includes Network Traffic Analysis for network flows
20	(Netflow, sflow, etc.), DNS and Proxy; primarily the identification of threats
21	through anomalous event detection using both supervised and unsupervised machine
22	learning.
23	
24	In order to support a broader set of use cases, Spot must be extended to collect
25	and analyze other common “event-oriented” data sources analyzed for cyber
26	threats, including but not limited to the following log types:
27	
28	-   Proxy
29	
30	-   Web server
31	
32	-   Operating system
33	
34	-   Firewall
35	
36	-   Intrusion Prevention/Detection (IDS/ IPS)
37	
38	-   Data Loss Prevention
39	
40	-   Active Directory / Identity Management
41	
42	-   User/Entity Behavior Analysis
43	
44	-   Endpoint Protection/Asset Management
45	
46	-   Network Metadata/Session and PCAP files
47	
48	-   Network Access Control
49	
50	-   Mail
51	
52	-   VPN
53	
54	-   etc..
55	
56	One of the biggest challenges organizations face today in combating cyber
57	threats is collecting and normalizing data from the myriad of security event
58	data sources (hundreds) in order to build the needed analytics. This often
59	results in the analytics being dependent upon the specific technologies used by
60	an organization to detect threats and prevents the needed flexibility and
61	agility to keep up with these ever-increasing (and complex) threats. Technology
62	lock-in is sometimes a byproduct of today’s status quo, as it’s extremely costly
63	to add new technologies (or replace existing ones) because of the downstream
64	analytic dependencies.
65	
66	To achieve the goal of extending Apache Spot (incubating) to support additional
67	use cases, it is necessary to create an open data model for the most relevant
68	security event and contextual data sources; Security event logs or alerts,
69	Network context, User details and information that comes from the endpoints or
70	any other console that are being use to manage the security / administration of
71	our endpoints. The presence of an open data model, which can be applied
72	“on-read” or “on-write”, in batch or stream, will allow for the separation of
73	security analytics from the specific data sources on which they are built. This
74	“separation of duties” will enable organizations to build analytics that are not
75	dependent upon specific technologies and provide the flexibility to change
76	underlying data sources and also provide segmentation of this information,
77	without impacting the analytics. This will also afford security vendors the
78	opportunity to build additional products on top of the Open Data Model to drive
79	new revenue streams and also to design new ways to detect threats and APT.
80	
81	**Apache Spot (incubating) Enabled Use Cases**
82	----------------------------------------------
