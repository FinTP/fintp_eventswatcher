fintp_eventswatcher
===================

Collects events related to messages and performance from all FinTP services	

Requirements
------------
- Xerces-C
- Xalan-C
- pthread
- **fintp_utils**
- **fintp_log**
- **fintp_transport**
- **fintp_udal**
- **fintp_base**

Build instructions
------------------
- On Unix-like systems, **fintp_eventswatcher** uses the GNU Build System (Autotools) so we first need to generate the configuration script using:


        autoreconf -fi
Now we must run:

        ./configure
        make

- For Windows, a Visual Studio 2010 solution is provided.

License
-------
- [GPLv3](http://www.gnu.org/licenses/gpl-3.0.html)

