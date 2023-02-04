weight: 4
bookCollapseSection: false
title: "Grammar"
---
# BF Grammar

BF Grammar -- Generated Productions & Alphabet
----------------------------------------------

BF Grammar for all developed Clusters: Cryptographic Store and Transfer Bugs Classes (_CRY), Data Type Bugs Classes (_DAT), Input/Outpu Bugs Classes (_INP), Memory Bugs Classes (_MEM):

`Bug := code_defect | specification_defect`

`code_defect = {Erroneous Code, Mismatched Operation, Missing Code, Wrong Code}`

`specification_defect = {Anonymous Scope, Inadequate Algorithm, Missing Modifier, Missing Qualifier, Modified Algorithm, Over-Restrictive Policy, Risky/Broken Algorithm, Under-Restrictive Policy, Weak Algorithm, Weak Protocol, Wrong Modifier, Wrong Qualifier, Wrong Scope}`

`Operation := ace_operation | dcl_operation | dom_operation | dos_operation | dvl_operation | dvr_operation | enc_operation | iex_operation | imp_operation | kmn_operation | mad_operation | mal_operation | mdl_operation | mus_operation | nrs_operation | tcm_operation | tcv_operation | tpr_operation | vrf_operation`

`dcl_operation = {Declare, Define}`

`dvl_operation = {Validate, Sanitize}`

`dvr_operation = {Verify, Correct}`

`mad_operation = {Initialize, Reposition, Reassign}`

`mal_operation = {Allocate, Extend, Reallocate-Extend}`

`mdl_operation = {Deallocate, Reduce, Reallocate-Reduce}`

`mus_operation = {DOS Operation}`

`nrs_operation = {Refer, Call}`

`tcm_operation = {Calculate, Evaluate}`

`tcv_operation = {Cast, Coerce}`

`enc_operation = {Encrypt, Decrypt}`

`vrf_operation = {Cryptographic Authenticate, Cryptographic Verify}`

`kmn_operation = {Generate/Select, Store, Distribute, Use, Destroy}`

`OperationAttribute := execution_space_attribute | mechanism_attribute | source_attribute`

`execution_space_attribute = {Admin, Bare-Metal, Kernel, Local, Userland}`

`mechanism_attribute = {Ad-hoc Bind, Asymmetric Algorithm, Bind, Data Type, Denylist, Digital Signature, Direct, Early Bind, Explicit, Format, Function, Generics, Hash Function + Random Numbers, Implicit, Lambda Expression, Late Bind, Length, Message Authentication Code (MAC), Method, Operator, Other Rules, Overloading, Overriding, Pass In, Pass Out, Procedure, Quantity, Range, Resolve, Safelist, Sequential, Simple, Symmetric Algorithm, Value}`

`source_attribute = {Codebase, Compiler/Interpreter, Standard Library, Third Party}`

`Fault := address_fault | data_fault | name_fault | size_fault | type_fault`

`data_fault = {Corrupted Data, Corrupted Policy Data, Flipped Sign, Forbidden Address, Hardcoded Address, Hardcoded Key, Over Range, Reference vs. Object, Single Owned Address, Tampered Data, Tampered Policy Data, Under Range, Unverified Data, Weak Cyphertext, Weak Key, Weak Other Keying Material, Wrong Argument, Wrong Index, Wrong Size Used}`

`type_fault = {Casted Pointer, Confused Subtype, Incomplete Type, Invalid Data, Mismatched Argument, Wrong Argument Type, Wrong Generic Type, Wrong Index Type, Wrong Object Type Resolved, Wrong Type, Wrong Type Resolved}`

`address_fault = {Dangling Pointer, NULL Pointer, Over Bounds Pointer, Under Bounds Pointer, Untrusted Pointer, Wild Pointer, Wrong Position Pointer}`

`size_fault = {Not Enough Memory Allocated}`

`name_fault = {Missing Overloaded Function, Missing Overridden Function, Wrong Function Resolved, Wrong Generic Function Bound, Wrong Object Resolved, Wrong Object Type Resolved, Wrong Overloaded Function Bound, Wrong Overridden Function Bound}`

`FaultAttribute := AddressAttribute | DataAttribute | NameAttribute | SizeAttribute | TypeAttribute`

`DataAttribute := cryptographic_data_kind_attribute | data_kind_attribute | sensitive_data_kind_attribute | sensitivity_attribute | state_attribute`

`TypeAttribute := type_kind_attribute`

`AddressAttribute := location_attribute | ownership_attribute`

`SizeAttribute := span_attribute`

`NameAttribute := entity_attribute`

`entity_attribute = {Data Type, Function, Namespace, Object}`

`data_kind_attribute = {Boolean, Numeric, Pointer, Text}`

`state_attribute = {Entered, In Use, Stored, Transferred, User Entered}`

`type_kind_attribute = {Primitive, Structure}`

`location_attribute = {/other/, Heap, Stack}`

`ownership_attribute = {None, Shared, Single}`

`span_attribute = {Huge, Litle, Moderate}`

`FinalError := access | data_security | injection | memory | type_compute`

`injection_final_error = {Command Injection, File Injection, Parameter Injection, Query Injection, Source Code Injection}`

`memory_final_error = {Buffer Overflow, Buffer Underflow, Double Free, Memory Leak, Memory Overflow, Not Cleared Object, NULL Pointer Dereference, Object Corruption, Type Confusion, Uninitialized Object, Uninitialized Pointer Dereference, Untrusted Pointer Dereference, Use After Free}`

`access_final_error = {Wrong Access Function, Wrong Access Object, Wrong Access Type}`

`type_compute_final_error = {Undefined}`
