**Install the collection**
```bash
ansible-galaxy collection install netbox.netbox
```

```bash
virtualenv .venv
source .venv/bin/activate
pip3 install pytz pynetbox ansible
```

`ansible-playbook main.yaml`

**Floor naming**

* **Floor B2** → Basement Level 2
* **Floor B1** → Basement Level 1
* **Floor G** → Ground Floor
* **Floor 1** → First Floor (above ground)
* **Floor 2** → Second Floor

Alternatives depending on context:

* **Level B2, Level B1, Level G, Level 1, Level 2**
  (very common in airports, malls, offices)
* **Storey B2, Storey B1, Storey G, Storey 1, Storey 2**
  (less common, but correct in British English)
* **Parking B2, Parking B1**
  (if only underground levels are for cars)

**Room naming**
| **BICSI TDMM Term**                   | **Function / Description**                                                                                                                       |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Entrance Facility (EF)**            | Building entry point where service provider cabling (WAN/ISP) terminates; includes demarcation point and grounding.                              |
| **Main Equipment Room (MER)**         | Central room housing building- or campus-wide telecom/network equipment (core routers, PBX, WAN termination, servers). Equivalent to MDF.        |
| **Equipment Room (ER)**               | Room for major telecom or IT equipment serving the building. MER is a special type of ER.                                                        |
| **Telecommunications Room (TR)**      | Floor-serving space with cross-connects, patch panels, and network switches; connects backbone cabling to horizontal cabling. Equivalent to IDF. |
| **Telecommunications Enclosure (TE)** | Small cabinet/enclosure serving a portion of a floor where a full TR isn’t needed.                                                               |
| **Data Center (DC)**                  | Specialized facility or space for high-density compute, storage, and networking equipment (defined in ANSI/BICSI-002).                           |
| **Work Area (WA)**                    | End-user space where devices (PCs, phones, APs) connect to the telecom cabling system.                                                           |