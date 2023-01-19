# watchtower
Node-RED flows for an IoT beach condition system.

These are exported Node-RED flows. 

The FinalCloud.json file is the Cloud flow, which runs an HTTP endpoint and connects to the Hawaii Beach Safety API. When commanded by the HTTP endpoint, the flow queries the REST API and parses the beach data for certain pre-selected beaches. The resulting information is the transmitted over the Internet to the nodes.

The FinalNode.json file, is the Node flow, which listens to incoming data from the Cloud flow. When updated, the Node updates its display  (a servo and LED) as appropriate.
