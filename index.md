This project is a port to Zeek of the [CICFlowMeter](https://github.com/ahlashkari/CICFlowMeter) project. Additional features have been integrated, while other duplicates have been removed. 

FlowMeter performs layer 3 and 4 network traffic analysis and generates a set of new features based on timing, volume and metadata. These features are ideal for developing models for traffic classification without using deep packet inspection. 

The advantage of using a standard network analysis framework like Zeek is that it is now possible to integrate the extraction of flow features in a standard solution. The identification of flows is therefore delegated to Zeek. Moreover, `FlowMeter` perform analysis on IPv6 flows too (currently CICFlowMeter do not support IPv6). 

This project adds the `flowmeter.zeek` script and the corresponding module with the name `FlowMeter`. Once activated, the module compute the features listed in the table below and write them into the `flowmeter.log` file. 
