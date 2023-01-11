---
weight: 2
title: "PRN"
---
# Pseudo-Random Number Bugs (PRN) CLASS

{{< hint danger >}}
**Note**

This class is still under development. The information will be updated soon.
{{< /hint >}}

### Definition

We define Pseudo-Random Number Bugs (PRN) as follows:

{{< definition >}}The software generated output does not satisfy all use-specific pseudo-randomness requirements{{< /definition >}}.

The output sequence is of random bits or numbers from a PRNG.

See also the [BF Model of Cryptographic Store or Transfer.](/Classes/_CRY/Model.md)

### Type

High (semantic).

### Taxonomy

Fig. 1 depicts PRN causes, attributes and consequences.

{{< img src="images/PRN.png" height="500" caption="Fig 1. Pseudo-Random Number Bugs (PRN) Class" >}}

### Attributes

**Function** – Conditioning, Mixing, Entropy Assessment, Seeding, Reseeding, Generate, Converting.

**Algorithm** – Concatenation, Hash Function, Block Cipher, XOR.

**Used For** – ASLR (Address Space Layout Randomization), Generation, Initialization, Input to Algorithm.

This is what the output sequence is used for. It could be used for ASLR, generation of passwords or cryptographic keying material (keys, nonces) , initialization of cryptographic primitives (e.g., an initialization vector for cipher block chaining mode of encryption; or a salt for hashing), or input to simulation, statistics, mathematics (e.g., Monte Carlo integration), or general algorithms.

**Pseudo-Randomness Requirement** – Unpredictability/ Indistinguishability, Prediction/ Backtracking Resistance, Sufficient Space Size, Use Specific Statistical Tests. This is the failed requirement.

### Related BF Classes

BF classes related to PRN are: [TRN](/Classes/_RND/TRN.md), [ENC](/Classes/_CRY/ENC.md), [VRF](/Classes/_CRY/VRF.md), [KMN](/Classes/_CRY/KMN.md), [IEX](/Old/Classes/IEX.md).

### Related CWEs and SFP

CWEs related to PRN are: [CWE-330](https://cwe.mitre.org/data/definitions/330.html), [CWE-331](https://cwe.mitre.org/data/definitions/331.html), [CWE-332](https://cwe.mitre.org/data/definitions/332.html), [CWE-334](https://cwe.mitre.org/data/definitions/334.html), [CWE-335](https://cwe.mitre.org/data/definitions/335.html), [CWE-336](https://cwe.mitre.org/data/definitions/336.html), [CWE-337](https://cwe.mitre.org/data/definitions/337.html), [CWE-338](https://cwe.mitre.org/data/definitions/338.html), [CWE-339](https://cwe.mitre.org/data/definitions/339.html), [CWE-340](https://cwe.mitre.org/data/definitions/340.html), [CWE-341](https://cwe.mitre.org/data/definitions/341.html),[CWE-342](https://cwe.mitre.org/data/definitions/342.html), [CWE-343](https://cwe.mitre.org/data/definitions/343.html).

The only related SFP cluster is SFP Primary Cluster: Predictability.

BF Descriptions of PRN Related CWEs are provided [here](https://docs.google.com/document/d/1ucIUmkGnm5gQj-7IHO3dCGguzVOmx15ukjzNWKwgZNA/edit).

### Application

Application examples can be found here: [CVE-2001-1141](/Examples/CVE-2001-1141.md), [CVE-2008-4107](/Examples/CVE-2008-4107.md). 

### References

\[1\] Bojanova, I., Yesha, Y., Black, P. E., Randomness Classes in Bugs Framework (BF): True-Random Number Bugs (TRN) and Pseudo-Random Number Bugs (PRN). IEEE COMPSAC 2018, NII, Tokyo, Japan. July 23-27, 2018.