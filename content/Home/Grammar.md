BF Grammar for all developed Clusters: Cryptographic Store and Transfer Bugs Classes (_CRY), Data Type Bugs Classes (_DAT), Input/Outpu Bugs Classes (_INP), Memory Bugs Classes (_MEM)

START := Vulnerability Converge

Vulnerability := Bug Operation Error

Error := Fault Operation Error | FinalError

Converge := Vulnerability Converge | Failure END


Bug := code_defect | specification_defect

code_defect = {Erroneous Code, Mismatched Operation, Missing Code, Wrong Code}

specification_defect = {Anonymous Scope, Inadequate Algorithm, Missing Modifier, Missing Qualifier, Modified Algorithm, Over-Restrictive Policy, Risky/Broken Algorithm, Under-Restrictive Policy, Weak Algorithm, Weak Protocol, Wrong Modifier, Wrong Qualifier, Wrong Scope}

Operation := ace_opr ACE_oa | dcl_opr DCL_oa | dom_opr DOM_oa | dos_opr DOS_oa | dvl_opr DVL_oa | dvr_opr DVR_oa | enc_opr ENC_oa | iex_opr IEX_oa | imp_opr IMP_oa | kmn_opr KMN_oa | mad_opr MAD_oa | mal_opr MAL_oa | mdl_opr MDL_oa | mus_opr MUS_oa | nrs_opr NRS_oa | tcm_opr TCM_oa | tcv_opr TCV_oa | tpr_opr TPR_oa | vrf_opr VRF_oa

dcl_opr = {Declare, Define}

dvl_opr = {Validate, Sanitize}

dvr_opr = {Verify, Correct}

mad_opr = {Initialize, Reposition, Reassign}

mal_opr = {Allocate, Extend, Reallocate-Extend}

mdl_opr = {Deallocate, Reduce, Reallocate-Reduce}

mus_opr = {DOS Operation}

nrs_opr = {Refer, Call}

tcm_opr = {Calculate, Evaluate}

tcv_opr = {Cast, Coerce}

enc_opr = {Encrypt, Decrypt}

vrf_opr = {Cryptographic Authenticate, Cryptographic Verify}

kmn_opr = {Generate/Select, Store, Distribute, Use, Destroy}

DVL_oa := DVL_execution_space | DVL_mechanism | DVL_source

DVR_oa := DVR_execution_space | DVR_mechanism | DVR_source

MAD_oa := MAD_execution_space | MAD_mechanism | MAD_source

MAL_oa := MAL_execution_space | MAL_mechanism | MAL_source

MUS_oa := MUS_execution_space | MUS_mechanism | MUS_source

MDL_oa := MDL_execution_space | MDL_mechanism | MDL_source

DCL_oa := DCL_execution_space | DCL_mechanism | DCL_source

NRS_oa := NRS_execution_space | NRS_mechanism | NRS_source

TCV_oa := TCV_execution_space | TCV_mechanism | TCV_source

TCM_oa := TCM_execution_space | TCM_mechanism | TCM_source

ENC_oa := ENC_execution_space | ENC_mechanism | ENC_source

VRF_oa := VRF_execution_space | VRF_mechanism | VRF_source

KMN_oa := KMN_execution_space | KMN_mechanism | KMN_source

execution_space_oa = {Admin, Bare-Metal, Kernel, Local, Userland}

mechanism_oa = {Ad-hoc Bind, Asymmetric Algorithm, Bind, Data Type, Denylist, Digital Signature, Direct, Early Bind, Explicit, Format, Function, Generics, Hash Function + Random Numbers, Implicit, Lambda Expression, Late Bind, Length, Message Authentication Code (MAC), Method, Operator, Other Rules, Overloading, Overriding, Pass In, Pass Out, Procedure, Quantity, Range, Resolve, Safelist, Sequential, Simple, Symmetric Algorithm, Value}

source_oa = {Codebase, Compiler/Interpreter, Standard Library, Third Party}

Operand := address | data | name | size | type

Fault := address_flt Address_fa | data_flt Data_fa | name_flt Name_fa | size_flt Size_fa | type_flt Type_fa

data_flt = {Corrupted Data, Corrupted Policy Data, Flipped Sign, Forbidden Address, Hardcoded Address, Hardcoded Key, Over Range, Reference vs. Object, Single Owned Address, Tampered Data, Tampered Policy Data, Under Range, Unverified Data, Weak Cyphertext, Weak Key, Weak Other Keying Material, Wrong Argument, Wrong Index, Wrong Size Used}

type_flt = {Casted Pointer, Confused Subtype, Incomplete Type, Invalid Data, Mismatched Argument, Wrong Argument Type, Wrong Generic Type, Wrong Index Type, Wrong Object Type Resolved, Wrong Type, Wrong Type Resolved}

address_flt = {Dangling Pointer, NULL Pointer, Over Bounds Pointer, Under Bounds Pointer, Untrusted Pointer, Wild Pointer, Wrong Position Pointer}

size_flt = {Not Enough Memory Allocated}

name_flt = {Missing Overloaded Function, Missing Overridden Function, Wrong Function Resolved, Wrong Generic Function Bound, Wrong Object Resolved, Wrong Object Type Resolved, Wrong Overloaded Function Bound, Wrong Overridden Function Bound}

Data_fa := cryptographic_data_kind_fa | data_kind_fa | sensitive_data_kind_fa | sensitivity_fa | state_fa

Type_fa := type_kind_fa

Address_fa := location_fa | ownership_fa

Size_fa := span_fa

Name_fa := entity_fa

entity_oa = {Data Type, Function, Namespace, Object}

data_kind_oa = {Boolean, Numeric, Pointer, Text}

state_oa = {Entered, In Use, Stored, Transferred, User Entered}

type_kind_oa = {Primitive, Structure}

location_oa = {/other/, Heap, Stack}

ownership_oa = {None, Shared, Single}

span_oa = {Huge, Litle, Moderate}

FinalError := access | data_security | injection | memory | type_compute

injection_final_error = {Command Injection, File Injection, Parameter Injection, Query Injection, Source Code Injection}

memory_final_error = {Buffer Overflow, Buffer Underflow, Double Free, Memory Leak, Memory Overflow, Not Cleared Object, NULL Pointer Dereference, Object Corruption, Type Confusion, Uninitialized Object, Uninitialized Pointer Dereference, Untrusted Pointer Dereference, Use After Free}

access_final_error = {Wrong Access Function, Wrong Access Object, Wrong Access Type}

type_compute_final_error = {Undefined}
