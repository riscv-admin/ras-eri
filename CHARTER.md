# RERI (RAS Error-record Register Interface) TG Charter

The RERI Task Group shall develop a specification to augment RAS features in RISC-V SOC hardware to standardize reporting and logging of errors by means of a memory-mapped register interface to enable error detection, provide the facility to log the detected errors (including their severity, nature, and location), and configuring means to report the error to a handler component. The specification shall support reporting attempts to consume corrupted data by an ultimate consumer component. Additionally, the specification shall support software-initiated error logging, reporting, and testing of error handlers. Lastly, the specification shall provide maximal flexibility to implement error handling and shall co-exist with RAS frameworks defined by other standards such as PCIe, CXL, etc.

The RERI specification shall not prescribe:

 - the level of reliability, availability, and serviceability in the system
 - methods for error detection and/or correction and testing of such methods
 - the behavior of the components on detecting the errors
 - behavior of components in the system that choose not to implement this specification

The RERI TG shall validate its specification by prototyping the behavior using QEMU and Linux.
