Python setup.py sdist service
=============================

This service creates a source distribution (sdist) from a Python project (containing a setup.py file)

Example _service file:

.. code-block:: xml

    <services>
      <service name="tar_scm" mode="disabled">
        <param name="url">git://github.com/kwwii/horizon.git</param>
        <param name="scm">git</param>
        <param name="package-meta">.git</param>
        <param name="versionformat">1.0.0</param>
        <param name="revision">grizzly-suse-ui</param>
      </service>
      <service name="python_sdist" mode="disabled">
        <param name="basename">horizon-*.tar</param>
      </service>
    </services>

