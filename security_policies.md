# AWS Security Policies

## Step 2: Firewall Rule Architecture

### 1. Do security groups support both "allow" and "deny" rules?

No. AWS Security Groups only support **allow** rules. They do not support explicit deny rules.

Traffic filtering works by:
- Allowing only the traffic explicitly permitted in the security group rules.
- Automatically denying all other traffic that is not allowed.

This follows the principle of least privilege by limiting access to only required services and ports.

---

### 2. Default Inbound and Outbound Traffic Behavior

#### Inbound Traffic
By default, all inbound traffic is denied unless explicitly allowed by a rule.

#### Outbound Traffic
By default, all outbound traffic is allowed unless outbound rules are restricted manually.

---

### 3. How Security Groups Are Applied

Security groups are applied externally to EC2 instances as virtual firewalls.

EC2 instances are not internally aware of the security groups attached to them.

A single security group can also be reused and attached to multiple EC2 instances.

---

# Step 3: Core Port Mapping Matrix

| Port Number | Protocol | Purpose |
|---|---|---|
| 22 | SSH | Secure remote administration for Linux servers |
| 21 | FTP | File Transfer Protocol used for transferring files |
| 80 | HTTP | Standard unencrypted web traffic |
| 443 | HTTPS | Secure encrypted web traffic |
| 3389 | RDP | Remote Desktop Protocol for Windows remote access |
