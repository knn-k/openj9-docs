<!--
* Copyright (c) 2017, 2023 IBM Corp. and others
*
* This program and the accompanying materials are made
* available under the terms of the Eclipse Public License 2.0
* which accompanies this distribution and is available at
* https://www.eclipse.org/legal/epl-2.0/ or the Apache
* License, Version 2.0 which accompanies this distribution and
* is available at https://www.apache.org/licenses/LICENSE-2.0.
*
* This Source Code may also be made available under the
* following Secondary Licenses when the conditions for such
* availability set forth in the Eclipse Public License, v. 2.0
* are satisfied: GNU General Public License, version 2 with
* the GNU Classpath Exception [1] and GNU General Public
* License, version 2 with the OpenJDK Assembly Exception [2].
*
* [1] https://www.gnu.org/software/classpath/license.html
* [2] https://openjdk.org/legal/assembly-exception.html
*
* SPDX-License-Identifier: EPL-2.0 OR Apache-2.0 OR GPL-2.0-only WITH Classpath-exception-2.0 OR GPL-2.0-only WITH OpenJDK-assembly-exception-1.0
-->

# What's new in version 0.41.0

The following new features and notable changes since version 0.40.0 are included in this release:

- [New binaries and changes to supported environments](#binaries-and-supported-environments)
- ![Start of content that applies to Java 21 (LTS) and later](cr/java21plus.png) [New `-XX:[+|-]ShowCarrierFrames` option added](#new-xx-showcarrierframes-option-added) ![End of content that applies to Java 21 (LTS) and later](cr/java_close_lts.png)

## Features and changes

### Binaries and supported environments

Eclipse OpenJ9&trade; release 0.41.0 supports OpenJDK 8, 11, and 17.

To learn more about support for OpenJ9 releases, including OpenJDK levels and platform support, see [Supported environments](openj9_support.md).

### ![Start of content that applies to Java 21 (LTS) and later](cr/java21plus.png) New `-XX:[+|-]ShowCarrierFrames` option added

A VM maintains multiple platform threads that are used as carrier threads to run the virtual threads. Although the virtual thread runs on a carrier thread, the stack trace of the virtual thread and its carrier thread are separate. You can use the `-XX:+ShowCarrierFrames` option to add the stack trace of the carrier thread in addition to the virtual thread stack trace to the `Throwable.getStackTrace()` method, if an exception occurs.

For more information, see [`-XX:[+|-]ShowCarrierFrames`](xxshowcarrierframes.md). ![End of content that applies to Java 21 (LTS) and later](cr/java_close_lts.png)

## Known problems and full release information

To see known problems and a complete list of changes between Eclipse OpenJ9 v0.40.0 and v0.41.0 releases, see the [Release notes](https://github.com/eclipse-openj9/openj9/blob/master/doc/release-notes/0.41/0.41.md).

<!-- ==== END OF TOPIC ==== version0.41.md ==== -->
