# Memory dump analysis

<<<<<<< HEAD
## Memory dump analysis

&lt;&lt;&lt;&lt;&lt;&lt;&lt; HEAD:forensics/memory-dump-analysis.md

## Start **searching** for **malware** inside the pcap. Use the **tools** mentioned in [**Malware Analysis**](https://github.com/TheShooter/hacktricks/tree/4cdf72ba217885f33024d77c382ee6da1fbdf3bc/forensics/basic-forensic-methodology/memory-dump-analysis/malware-analysis.md).

Start **searching** for **malware** inside the pcap. Use the **tools** mentioned in [**Malware Analysis**](../malware-analysis.md).
=======
Start **searching **for **malware **inside the pcap. Use the **tools **mentioned in [**Malware Analysis**](../malware-analysis.md).
>>>>>>> 72cbd88461ed0e65da5433596050dd2ecb643f6b

> > > > > > > upstream/master:forensics/basic-forensic-methodology/memory-dump-analysis/README.md

### [Volatility](volatility-examples.md)

The premiere open-source framework for memory dump analysis is [Volatility](volatility-examples.md). Volatility is a Python script for parsing memory dumps that were gathered with an external tool (or a VMware memory image gathered by pausing the VM). So, given the memory dump file and the relevant "profile" (the OS from which the dump was gathered), Volatility can start identifying the structures in the data: running processes, passwords, etc. It is also extensible using plugins for extracting various types of artifact.\
From: [https://trailofbits.github.io/ctf/forensics/](https://trailofbits.github.io/ctf/forensics/)

### Mini dump crash report

When the dump is small (just some KB, maybe a few MB) the it's probably a mini dump crash report and not a memory dump.

![](<../../../.gitbook/assets/image (216).png>)

If you hat Visual Studio installed, you can open this file and bind some basic information like process name, architecture, exception info and modules being executed:

![](<../../../.gitbook/assets/image (217).png>)

You can also load the exception and see the decompiled instructions

![](<../../../.gitbook/assets/image (219).png>)

![](<../../../.gitbook/assets/image (218).png>)

Anyway Visual Studio isn't the best tool to perform a analysis in depth of the dump.

<<<<<<< HEAD
You should **open** it using **IDA** or **Radare** to inspection it in **depth**.
=======
You should **open **it using **IDA **or **Radare **to inspection it in **depth**.


>>>>>>> 72cbd88461ed0e65da5433596050dd2ecb643f6b

