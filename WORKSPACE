# -*- python -*-

# Copyright 2023 mjbots Robotic Systems, LLC.  info@mjbots.com
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

workspace(name = "com_github_mjbots_rules_mbed")

BAZEL_VERSION = "5.4.1"
BAZEL_VERSION_SHA = "5d90515f84b5ee1fd6ec22ee9e83103e77ed1a907ee5eec198fef3a5b45abf13"

load("//:rules.bzl", "mbed_register")
load("//tools/workspace/mbed:repository.bzl", "mbed_repository")

mbed_register()

mbed_repository(
    name = "com_github_ARMmbed_mbed-os_g474",
    target = "targets/TARGET_STM/TARGET_STM32G4/TARGET_STM32G474xE/TARGET_NUCLEO_G474RE",
    config = {
        "MBED_CONF_RTOS_PRESENT": "0",
        "DEVICE_STDIO_MESSAGES": "0",
        "MBED_CONF_TARGET_CONSOLE_UART": "1",
    },
)
