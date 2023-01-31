weight: 4
bookCollapseSection: false
title: "Grammar"
---
# BF Grammar

BF Grammar for all developed Clusters: Data Type Bugs Classes (_DAT), Input/Outpu Bugs Classes (_INP), Memory Bugs Classes (_MEM)

(need to add Attributes)

`START := Vulnerability Converge`

`Vulnerability := Defect Operation Error`

`Error := Fault Operation Error | FinalError`

`Converge := Vulnerability Converge | Failure END`


`Operation := dcl_operation | dvl_operation | dvr_operation | mad_operation | mal_operation | mdl_operation | mus_operation | nrs_operation | tcm_operation | tcv_operation`

`Operand := address | data | name | size | type`


`Defect := code | specification`

`Fault := address_fault | data_fault | name_fault | size_fault | type_fault`

`FinalError := access | injection | memory | type_compute`


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


`code_defect = {Erroneous Code, Mismatched Operation, Missing Code, Wrong Code}`

`specification_defect = {Anonymous Scope, Corrupted Policy Data, Missing Modifier, Missing Qualifier, Over-Restrictive Policy, Tampered Policy Data, Under-Restrictive Policy, Wrong Modifier, Wrong Qualifier, Wrong Scope}`


`data_fault = {Corrupted Data, Flipped Sign, Forbidden Address, Hardcoded Address, Over Range, Reference vs. Object, Single Owned Address, Tampered Data, Under Range, Wrong Argument, Wrong Index, Wrong Size Used}`

`type_fault = {Casted Pointer, Confused Subtype, Incomplete Type, Invalid Data, Mismatched Argument, Wrong Argument Type, Wrong Generic Type, Wrong Index Type, Wrong Object Type Resolved, Wrong Type, Wrong Type Resolved}`

`address_fault = {Dangling Pointer, NULL Pointer, Over Bounds Pointer, Under Bounds Pointer, Untrusted Pointer, Wild Pointer, Wrong Position Pointer}`

`size_fault = {Not Enough Memory Allocated}`

`name_fault = {Missing Overloaded Function, Missing Overridden Function, Wrong Function Resolved, Wrong Generic Function Bound, Wrong Object Resolved, Wrong Object Type Resolved, Wrong Overloaded Function Bound, Wrong Overridden Function Bound}`


`injection_final_fault = {Command Injection, File Injection, Parameter Injection, Query Injection, Source Code Injection}`

`memory_final_fault = {Buffer Overflow, Buffer Underflow, Double Free, Memory Leak, Memory Overflow, Not Cleared Object, NULL Pointer Dereference, Object Corruption, Type Confusion, Uninitialized Object, Uninitialized Pointer Dereference, Untrusted Pointer Dereference, Use After Free}`

`access_final_fault = {Wrong Access Function, Wrong Access Object, Wrong Access Type}`

`type_compute_final_fault = {Undefined}`
