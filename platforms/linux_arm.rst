..  Copyright (c) 2014-present PlatformIO <contact@platformio.org>
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
       http://www.apache.org/licenses/LICENSE-2.0
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

.. _platform_linux_arm:

Linux ARM
=========

:Configuration:
  :ref:`projectconf_env_platform` = ``linux_arm``

Linux ARM is a Unix-like and mostly POSIX-compliant computer operating system (OS) assembled under the model of free and open-source software development and distribution. Using host OS (Mac OS X, Linux ARM) you can build native application for Linux ARM platform.

For more detailed information please visit `vendor site <http://platformio.org/platforms/linux_arm?utm_source=platformio&utm_medium=docs>`_.

.. contents:: Contents
    :local:
    :depth: 1


Examples
--------

Examples are listed from `Linux ARM development platform repository <https://github.com/platformio/platform-linux_arm/tree/master/examples?utm_source=platformio&utm_medium=docs>`_:

* `wiringpi-blink <https://github.com/platformio/platform-linux_arm/tree/master/examples/wiringpi-blink?utm_source=platformio&utm_medium=docs>`_
* `wiringpi-serial <https://github.com/platformio/platform-linux_arm/tree/master/examples/wiringpi-serial?utm_source=platformio&utm_medium=docs>`_

Stable and upstream versions
----------------------------

You can switch between `stable releases <https://github.com/platformio/platform-linux_arm/releases>`__
of Linux ARM development platform and the latest upstream version using
:ref:`projectconf_env_platform` option in :ref:`projectconf` as described below.

Stable
~~~~~~

.. code-block:: ini

    ; Latest stable version
    [env:latest_stable]
    platform = linux_arm
    board = ...

    ; Custom stable version
    [env:custom_stable]
    platform = linux_arm@x.y.z
    board = ...

Upstream
~~~~~~~~

.. code-block:: ini

    [env:upstream_develop]
    platform = https://github.com/platformio/platform-linux_arm.git
    board = ...


Packages
--------

.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - `framework-artik-sdk <http://www.artik.io?utm_source=platformio&utm_medium=docs>`__
      - ARTIK SDK is a C/C++ SDK targeting Samsung ARTIK platforms

    * - `framework-wiringpi <http://wiringpi.com?utm_source=platformio&utm_medium=docs>`__
      - GPIO Interface library for the Raspberry Pi

    * - `toolchain-gccarmlinuxgnueabi <https://gcc.gnu.org?utm_source=platformio&utm_medium=docs>`__
      - GCC for Linux ARM GNU EABI

Frameworks
----------
.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - :ref:`framework_artik-sdk`
      - ARTIK SDK is a C/C++ SDK targeting Samsung ARTIK platforms. It exposes a set of APIs to ease up development of applications. These APIs cover hardware buses such as GPIO, SPI, I2C, UART, connectivity links like Wi-Fi, Bluetooth, Zigbee, and network protocols such as HTTP, Websockets, MQTT, and others.

    * - :ref:`framework_wiringpi`
      - WiringPi is a GPIO access library written in C for the BCM2835 used in the Raspberry Pi. It's designed to be familiar to people who have used the Arduino "wiring" system.

Boards
------

.. note::
    * You can list pre-configured boards by :ref:`cmd_boards` command or
      `PlatformIO Boards Explorer <https://platformio.org/boards>`_
    * For more detailed ``board`` information please scroll tables below by
      horizontal.

Raspberry Pi
~~~~~~~~~~~~

.. list-table::
    :header-rows:  1

    * - ID
      - Name
      - Debug
      - MCU
      - Frequency
      - Flash
      - RAM
    * - ``raspberrypi_1b``
      - `Raspberry Pi 1 Model B <https://www.raspberrypi.org?utm_source=platformio&utm_medium=docs>`_
      - No
      - BCM2835
      - 700MHz
      - 512MB
      - 512MB
    * - ``raspberrypi_2b``
      - `Raspberry Pi 2 Model B <https://www.raspberrypi.org?utm_source=platformio&utm_medium=docs>`_
      - No
      - BCM2836
      - 900MHz
      - 1GB
      - 1GB
    * - ``raspberrypi_3b``
      - `Raspberry Pi 3 Model B <https://www.raspberrypi.org?utm_source=platformio&utm_medium=docs>`_
      - No
      - BCM2837
      - 1200MHz
      - 1GB
      - 1GB
    * - ``raspberrypi_zero``
      - `Raspberry Pi Zero <https://www.raspberrypi.org?utm_source=platformio&utm_medium=docs>`_
      - No
      - BCM2835
      - 1000MHz
      - 512MB
      - 512MB

RushUp
~~~~~~

.. list-table::
    :header-rows:  1

    * - ID
      - Name
      - Debug
      - MCU
      - Frequency
      - Flash
      - RAM
    * - ``kitra_520``
      - `RushUp Kitra 520 <https://www.rushup.tech/kitra?utm_source=platformio&utm_medium=docs>`_
      - No
      - EXYNOS3250
      - 1000MHz
      - 4GB
      - 512MB

Samsung
~~~~~~~

.. list-table::
    :header-rows:  1

    * - ID
      - Name
      - Debug
      - MCU
      - Frequency
      - Flash
      - RAM
    * - ``artik_1020``
      - `Samsung ARTIK 1020 <https://www.artik.io?utm_source=platformio&utm_medium=docs>`_
      - No
      - EXYNOS5422
      - 1500MHz
      - 16GB
      - 2GB
    * - ``artik_520``
      - `Samsung ARTIK 520 <https://www.artik.io?utm_source=platformio&utm_medium=docs>`_
      - No
      - EXYNOS3250
      - 1000MHz
      - 4GB
      - 512MB
    * - ``artik_530``
      - `Samsung ARTIK 530 <https://www.artik.io?utm_source=platformio&utm_medium=docs>`_
      - No
      - S5P4418
      - 1200MHz
      - 4GB
      - 512MB
    * - ``artik_710``
      - `Samsung ARTIK 710 <https://www.artik.io?utm_source=platformio&utm_medium=docs>`_
      - No
      - S5P6818
      - 1400MHz
      - 4GB
      - 1GB
