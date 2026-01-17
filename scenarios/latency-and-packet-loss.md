# Monitoring Scenario: Latency and Packet Loss

## Scenario Overview
This scenario documents the detection and investigation of increased network latency and intermittent packet loss affecting end-user connectivity.

The goal is to demonstrate how performance degradation is identified through monitoring and validated before escalation.

---

## Initial Detection
The monitoring system detects elevated latency and packet loss on a monitored network link.

Observed symptoms include:
- Increased round-trip time (RTT)
- Intermittent packet loss exceeding baseline thresholds
- User-reported slowness and timeouts

---

## Metrics Involved
- **Latency (ICMP RTT):** Measures response time between monitoring system and network device
- **Packet Loss:** Indicates dropped packets over a monitored path
- **Availability:** Confirms the device remains reachable despite degradation

---

## Alert Conditions
Alerts are triggered when:
- Latency exceeds acceptable thresholds for a sustained period
- Packet loss exceeds a defined percentage threshold
- Conditions persist beyond transient fluctuation windows

Thresholds are tuned to avoid alert fatigue caused by short-lived spikes.

---

## Investigation Process
1. Verify alert accuracy by checking historical performance trends
2. Confirm packet loss using ICMP and interface statistics
3. Correlate alerts with recent network changes or maintenance
4. Identify whether the issue is localized or widespread

---

## Operational Response
- Acknowledge the alert and begin investigation
- Notify stakeholders if user impact is confirmed
- Escalate to network engineering or service provider if required
- Monitor metrics closely during remediation

---

## Resolution and Follow-Up
Once latency and packet loss return to baseline:
- Confirm service stability
- Clear active alerts
- Document findings and resolution steps
- Review thresholds to ensure continued accuracy

---

## Key Takeaways
- Performance issues often occur without full outages
- Monitoring latency and packet loss provides early warning
- Proper threshold tuning reduces false positives
- Structured response improves resolution time
