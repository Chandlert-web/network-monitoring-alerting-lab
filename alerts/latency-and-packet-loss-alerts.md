# Alert Definitions: Latency and Packet Loss

## Overview
This document defines alert thresholds and logic for detecting network latency and packet loss events.

Alerts are designed to be actionable, meaningful, and resistant to transient network fluctuations.

---

## Latency Alert

**Trigger Condition:**
- Average latency exceeds baseline threshold for a sustained period

**Example Threshold:**
- Latency > 100 ms for 5 consecutive polling intervals

**Rationale:**
Short latency spikes are common and often harmless. Sustained elevation indicates congestion or upstream issues requiring investigation.

---

## Packet Loss Alert

**Trigger Condition:**
- Packet loss exceeds defined percentage for a sustained duration

**Example Threshold:**
- Packet loss > 2% for 3 consecutive polling intervals

**Rationale:**
Packet loss at low percentages can already impact user experience. Sustained loss warrants escalation.

---

## Combined Alert Logic
Latency and packet loss alerts are correlated when possible to reduce false positives.

Examples:
- Latency increase without packet loss may indicate congestion
- Packet loss with normal latency may indicate physical layer issues

Correlated alerts provide better diagnostic context.

---

## Alert Severity Levels

- **Warning:**  
  Threshold breached briefly or marginally  
  Used for awareness and trend monitoring

- **Critical:**  
  Threshold breached consistently  
  Requires immediate investigation and response

---

## Alert Handling Workflow
1. Alert triggers and is acknowledged
2. Engineer validates metrics against historical trends
3. User impact is assessed
4. Escalation occurs if impact is confirmed
5. Resolution steps are documented

---

## Alert Fatigue Prevention
- Thresholds tuned to sustained conditions
- Alerts correlated across metrics
- Warning vs critical severity separation
- Periodic review of alert effectiveness

---

## Summary
Effective alerting balances sensitivity with stability, ensuring alerts drive action rather than noise.
