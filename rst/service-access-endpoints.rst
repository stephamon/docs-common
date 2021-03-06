.. _service-access-endpoints:

Service access endpoints
~~~~~~~~~~~~~~~~~~~~~~~~

The |product name| service is a regionalized service. The user of the service is 
therefore responsible for selecting the appropriate regional endpoint to ensure access to 
servers, networks, or other Cloud services.

.. tip:: To help you decide which regionalized endpoint to use, read about
   :kc-article:`special considerations<about-regions>` for choosing a data center.

If you are working with cloud services that are in one of the Rackspace data centers, using 
the ServiceNet endpoint in the same data center has no network costs and provides a faster 
connection. ServiceNet is the data center internet network. In your authentication response 
service catalog, it is listed as InternalURL. If you are working with services that are not 
in one of the Rackspace data centers, you must use a public endpoint to connect. In your 
authentication response, public endpoints are listed as publicURL. If you are working with 
services in multiple data centers or have a mixed environment where you have services both 
in your data centers and in Rackspace data centers, use a public endpoint because it is 
accessible from all the servers in the different environments.

.. note::
   You should copy the base URLs directly from the catalog rather than trying to construct 
   them manually.

   Rackspace Cloud Identity returns a service catalog, which includes regional endpoints 
   with your account ID. Your account ID, also known as project ID or tenant ID, refers to 
   your Rackspace account number.

.. tip::
   If you do not know your account ID or which data center you are working in, you can find 
   that information in your :mycloud:`Cloud Control Panel<>`.
