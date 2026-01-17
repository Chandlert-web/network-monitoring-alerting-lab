# Core Network Monitoring Metrics

## Overview
This document defines the core network performance metrics monitored in the Network Monitoring & Alerting Lab.

These metrics provide visibility into network health, performance, and availability and are commonly used in enterprise and service provider environments.

---

## Latency
**Description:**  
Latency measures the round-trip time (RTT) between the monitoring system and a network device.

**Why It Matters:**  
High latency can indicate congestion, routing issues, or upstream provider problems and often impacts application performance before outages occur.

**Monitoring Method:**  
- ICMP polling
- Historical trend analysis

---

## Packet Loss
**Description:**  
Packet loss represents the percentage of packets that fail to reach their destination.

**Why It Matters:**  
Even small amounts of packet loss can significantly degrade application performance, especially for real-time services.

**Monitoring Method:**  
- ICMP packet loss measurement
- Interface error counters

---

## Availability
**Description:**  
Availability measures whether a device or service is reachable over time.

**Why It Matters:**  
Availability confirms device uptime but does not reflect performance quality.

**Monitoring Method:**  
- ICMP reachability checks
- SNMP status polling

---

## Interface Utilization
**Description:**  
Interface utilization tracks bandwidth usage on network interfaces.

**Why It Matters:**  
High utilization can lead to congestion, increased latency, and packet loss.

**Monitoring Method:**  
- SNMP interface counters
- Trend-based analysis

---

## Error Rates
**Description:**  
Error rates track packet errors on network interfaces.

**Why It Matters:**  
Increasing error rates may indicate physical layer issues, duplex mismatches, or failing hardware.

**Monitoring Method:**  
- SNMP error counters
- Interface statistics review

---

## Summary
Monitoring these metrics together provides a complete view of network health, allowing early detection of performance degradation and proactive response.
