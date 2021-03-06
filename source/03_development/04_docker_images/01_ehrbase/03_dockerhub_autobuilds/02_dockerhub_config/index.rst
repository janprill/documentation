Docker Hub Configuration
------------------------

.. note:: This part serves only as a reference and does not have to be repeated - it describes what was needed to do to configure automated Docker image builds on Docker Hub.


1. Create a Dockerfile in root of Github repository
2. Login to Docker Hub (docker.com) with the tech-user
3. Login to Github as the "real" owner of the Organisation
4. Connect the "real" owner to Docker Hub granting access to EHRbase Organisation to enable Autobuilds

.. image:: images/dockerhub_config_1.png
   :target: images/dockerhub_config_1.png
   :alt: Connect Docker Hub with your Github Org

.. warning:: It is not sufficient to connect the tech-user although he has owner privileges in EHRbase Organisation. Once the connection by "real" owner is established everything else can be configured with the tech-user login to Docker Hub (docker.com)

.. image:: images/dockerhub_config_2.png
   :target: images/dockerhub_config_2.png
   :alt: Use the real owner of the Github Org or repository to establish connection

5. Go to Builds / Configure Automated Builds

.. image:: images/dockerhub_config_3.png
   :target: images/dockerhub_config_3.png
   :alt: Go to Builds and then to Configure Automated Builds


6. Set Up Build Rules

.. image:: images/dockerhub_config_4.png
   :target: images/dockerhub_config_4.png
   :alt: Set up the build rules