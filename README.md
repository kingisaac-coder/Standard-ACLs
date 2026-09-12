# Standard-ACLs
Cisco Packet Tracer labs focused on configuring and applying standard IPv4 Access Control Lists (ACLs) to control network traffic based on source IP addresses.

# Standard Access Control List (ACL)

## 📖 Overview

This lab focused on configuring and applying Standard Access Control Lists (ACLs) on Cisco routers to control network traffic.

The lab provided hands-on experience creating ACL rules, controlling access based on source IPv4 addresses, applying ACLs to router interfaces, and verifying that traffic was permitted or denied according to the configured security policy.

## 🎯 Objectives

The lab was designed to:

* Understand the purpose of Access Control Lists.
* Configure a Standard IPv4 ACL.
* Permit or deny traffic based on source IP addresses.
* Apply an ACL to a router interface.
* Understand ACL processing and rule order.
* Verify ACL configuration and operation.
* Test permitted and denied traffic.
* Troubleshoot ACL-related connectivity issues.

## 🧠 Concepts Practiced

* Access Control Lists (ACLs)
* Standard ACLs
* IPv4 source-address filtering
* `permit` and `deny` statements
* ACL sequence/order
* Implicit deny
* Inbound and outbound ACL application
* Traffic filtering
* Network security
* ACL troubleshooting

## 🛠️ Tools Used

* Cisco Packet Tracer
* Cisco IOS CLI

## ⚙️ Configuration

A Standard ACL was created on the router to control traffic based on the source IPv4 address of network devices.

The ACL contained permit and/or deny statements defining which source addresses were allowed to access a particular network or service.

After creating the ACL, it was applied to the appropriate router interface in the required direction.

## 🧪 Verification & Testing

The ACL configuration was verified using commands such as:

```text
show access-lists
show ip access-lists
show running-config
```

Connectivity was tested using:

```text
ping <destination-ip>
```

Tests were performed from permitted and restricted hosts to confirm that the ACL was enforcing the intended access-control policy.

## 🔍 Troubleshooting

Common ACL issues investigated during the lab included:

* Applying the ACL to the wrong interface.
* Applying the ACL in the wrong direction.
* Incorrect source IP addresses.
* Incorrect permit/deny statements.
* ACL rules being placed in the wrong order.
* Forgetting the implicit deny behavior.
* Blocking traffic unintentionally.

Troubleshooting involved checking the ACL configuration, interface configuration, ACL counters, and performing connectivity tests from different hosts.

## 🔐 Security Concepts

Standard ACLs provide a basic method of controlling network traffic by filtering packets according to their **source IPv4 address**.

ACLs are processed sequentially, meaning the order of entries can affect the final result. Standard ACLs also have an implicit `deny` at the end of the ACL, making careful rule design important.

ACLs are an important foundation for understanding network access control and router-based traffic filtering.

## ✅ Outcome

Successfully configured and applied a Standard IPv4 ACL, verified its operation, and demonstrated how source-based traffic filtering can be used to control network access.

## 📚 Skills Demonstrated

* Cisco IOS CLI
* Standard IPv4 ACL configuration
* Source IP filtering
* Traffic control
* Interface ACL application
* ACL verification
* Network security fundamentals
* Connectivity testing
* Network troubleshooting
