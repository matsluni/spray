.. _-get-:

get
===

Matches requests with HTTP method ``GET``.

Signature
---------

.. includecode:: /../spray-routing/src/main/scala/spray/routing/directives/MethodDirectives.scala
   :snippet: get

Description
-----------

This directive filters the incoming request by its HTTP method. Only requests with
method ``GET`` are passed on to the inner route. All others are rejected with a
``MethodRejection``, which is translated into a ``405 Method Not Allowed`` response
by the default :ref:`RejectionHandler`.


Example
-------

.. includecode:: ../code/docs/directives/MethodDirectivesExamplesSpec.scala
  :snippet: get-method
