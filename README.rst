.. code:: bash

   docker-compose up

.. code:: bash

   cd plone-4
   buildout
   bin/instance fg
   # Create new Plone site with id Plone

   ./bin/instance -OPlone run bin/transmogrify plone.export plone.analyze --overrides=overrides.cfg

.. code:: bash

   cd plone-5
   buildout
   bin/instance fg
   # Create new Plone site with id Plone and remove its contents

   ./bin/exportimport -OPlone run bin/transmogrify plone.import --overrides=overrides.cfg
