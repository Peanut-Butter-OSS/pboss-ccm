The ccm-model module contains the shared domain model and related XML schemas and JSON files that specify the strcuture of information in the system.

It will be deployed as a separate jar to be included in all system components.

The ccm-model module will take its version from the pboss-ccm project

Any subsystem-specific "model" classes should still be defined inside the subsystem module.

Here is  a quick overview of each of the packages:

- com.eightbiplatoon.c3m.model.api
	- Generic api classes for the Eminent bulk SMS solution
	- It would make sense to continue using this pacakges for classes that will be reused in all APIs (such as request and response headers.

- com.eightbiplatoon.c3m.model.bulk_cic_svc
	- Service request and response definitions for the Eminent bulk SMS solution

- com.eightbiplatoon.c3m.model.dis_request_info_svc
	- Service request and response definition for the query service which was never fully implemented

- com.eightbiplatoon.c3m.model.domain
	- Generic classes as developed for the Eminent bulk SMS solution

- com.eightbiplatoon.c3m.model.request
	- The structure to be used by the request subsystem as developed for the final system

- com.eightbiplatoon.c3m.model.runtime_strcuture
	- The original structure as planned for the first Mule implementation.
	- This defines the structure of a CIC from the perspective of C3M, i.e. what we get from clients will look different.