# SOC Lab – Test Scenarios

## Scenario 1: Multiple Failed Login Attempts
- **Objective:** Detect repeated failed Windows login attempts.
- **Windows Event ID:** 4625
- **Expected result:** Splunk identifies repeated failures associated with an account.

## Scenario 2: Successful Login
- **Objective:** Identify successful Windows logins.
- **Windows Event ID:** 4624
- **Expected result:** Splunk records the successful login event.

## Scenario 3: Account Lockout
- **Objective:** Identify an account locked after repeated failed logins.
- **Windows Event ID:** 4740
- **Expected result:** Splunk identifies the account lockout event.

## Scenario 4: Suspicious Process Execution
- **Objective:** Monitor selected process creation events.
- **Source:** Sysmon Operational Log
- **Expected result:** Splunk records process execution details for investigation.

## Safety
All testing will use authorised, controlled activity on the local lab machine.