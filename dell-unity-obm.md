### Dell Unity

    Package Source : platformdxc-generic/edgex-mf/dxc/cp/snmp/DXC_OBM_Dell_Unity_Storage_Trap_Monitor_(1.00).zip

If disccovery is not enabled, the CIs need to be created manually. For the list of CIs (which need to be created) reach out to respective team (In this case Dell Unity) and request for CIs 

**[See Pre-requisites for SNMP Traps](https://github.dxc.com/pages/Innovation-Automation/edgex_documentation/User_Guides/monitoring/obm/policy_docs/policy_docs_traps/#monitoring-prerequisites)**

<b> Please Note </b>

    Even after that traps may bring some compound or default CI names which may not be in shared CI list. 
    Therefore rule should set in ServiceNow to catch any Dell Unity events with default CI and assign to Dell Unity team for that client

Traps are categorised as below -


| MIB|Enterprise ID:|Generic ID|Specific ID|Severity|Confdition name |Event Title |
| ----- | ----- | ------ | ----- | ----- | ------ | ------ |
DellUnity|.1.3.6.1.4.1.1139.103.1.18.2|6|0|critical|unityGenericTrapEmergency|Dell Unity - System is unusable - <$3>:<$4>
DellUnity|.1.3.6.1.4.1.1139.103.1.18.2|6|1|critical|unityGenericTrapAlert|Dell Unity -  Action needs to be taken immediately - <$3>:<$4>
DellUnity|.1.3.6.1.4.1.1139.103.1.18.2|6|2|critical|unityGenericTrapCritical|Dell Unity - The system is in critical condition - <$3>:<$4>
DellUnity|.1.3.6.1.4.1.1139.103.1.18.2|6|3|major|unityGenericTrapError|Dell Unity - There is an error in the system - <$3>:<$4>
DellUnity|.1.3.6.1.4.1.1139.103.1.18.2|6|4|minor|unityGenericTrapWarning|Dell Unity - There is a warning condition in the system - <$3>:<$4>
DellUnity|.1.3.6.1.4.1.1139.103.1.18.2|6|5|warning|unityGenericTrapNotice|Dell Unity - There is a normal but significant condition in the system - <$3>:<$4>
DellUnity|.1.3.6.1.4.1.1139.103.1.18.2|6|6|warning|unityGenericTrapInformational|Dell Unity - There is an informational message - <$3>:<$4>
DellUnity|.1.3.6.1.4.1.1139.103.1.18.2|6|7|warning|unityGenericTrapDebug|Dell Unity - There is a debug-level message - <$3>:<$4>



<b> Details of the Variables </b>

   <$3> : Unity trap symptom ID

   <$4> : Unity trap syptom text