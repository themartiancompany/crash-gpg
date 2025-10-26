..
   SPDX-License-Identifier: AGPL-3.0-or-later

   ----------------------------------------------------------------------
   Copyright © 2024, 2025  Pellegrino Prevete

   All rights reserved
   ----------------------------------------------------------------------

   This program is free software: you can redistribute it and/or modify
   it under the terms of the GNU Affero General Public License as published by
   the Free Software Foundation, either version 3 of the License, or
   (at your option) any later version.

   This program is distributed in the hope that it will be useful,
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU Affero General Public License for more details.

   You should have received a copy of the GNU Affero General Public License
   along with this program.  If not, see <https://www.gnu.org/licenses/>.


==================
libcrash-gpg
==================

-----------------------------------------------------------
Crash GNU Privacy Guard Library
-----------------------------------------------------------
:Version: libcrash-gpg |version|
:Manual section: 1

Synopsis
========


..  code-block:: bash

  _bin="$( \
    dirname \
      "$( \
        command \
          -v \
  	  "env")")"
  _lib="$( \
    realpath \
      "${_bin}/../lib")"
  _crash_gpg="${_lib}/libcrash-gpg/crash-gpg"
  _sourced \
    "${_crash_gpg}" 2>/dev/null || \
    source \
      "${_crash_gpg}"

Description
===========

Bash library providing useful functions
to interact with GNU Privacy Guard.

An example application using
the library is GPG Key Info
(*gpg-key-info*).

The Ethereum Virtual Machine GNU
Privacy Guard [1]_ (*evm-gpg*)
reference implementation by
The Martian Company
also uses the Crash GPG library,
so it is an essential
component in the Ethereum
GPG stack and for all applications
using it, such as
as the EVM OpenPGP Key Server [2]_,
the EVM Contracts Source Index [3]_,
the Ur [4]_ uncensorable Life
and DogeOS user repository and application
store reference implementation.

Crash GPG is a core component of the
Human Instrumentality Project (HIP).


Bugs
====

https://github.com/themartiancompany/crash-gpg/-/issues


Copyright
=========

Copyright Pellegrino Prevete. AGPL-3.0.


See also
========

* libcrash-bash
* libcrash-js


External Resources
===================

.. [1]  `Ethereum Virtual Machine GNU Privacy Guard`_
.. [2]  `Ethereum Virtual Machine OpenPGP Key Server`_
.. [3]  `Ethereum Virtual Machine Contracts Source Index`_
.. [4]  `Ur`_

.. include:: variables.rst
