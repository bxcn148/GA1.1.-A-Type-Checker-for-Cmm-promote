Download link :https://programming.engineering/product/ga1-1-a-type-checker-for-cmm-promote/


# GA1.1.-A-Type-Checker-for-Cmm-promote
GA1.1. A Type Checker for Cmm – promote
A Type Checker for Cmm Supporting Implicit Type Coercions and Operator Overloading – Promotion

The purpose of this question is to help the student master:

• Understand the concept of promotion of types as used in C

171 Open workspace

Using VSCode – General Instructions

Problem Background

Problem

• Write a function numeric_type_less : numeric_type —> numeric_type —> boot that implements the ordering:

char < jut < float

• Based on the ordering above, write the function val max_numeric_type : numeric_type —> numeric_type —> numeric_type = <fun>

• Write the function val promote_to_numeric_type : (typed_monop, typed_binop) exp * numeric_type —> numeric_type —> (typed_monop, typed_binop) exp option = <fun> that is given first a pair of an expression to be promoted with the assumed type of that expression to be promoted, and then the type to which the expression is to be promoted. It returns the expression resulting from applying to the given expression the needed sequence of type coercions, given as monadic operators, such as IntOf C ha r. If no valid promotion exists, > the function should return None. Note: This function can only meaningfully be applied to expressions of a numeric type.

• Write the function val promote : (typed_monop, typed_binop) exp * exp_type —> exp_type —> (typed_monop, typed_binop) exp option = <fun> The difference between p romote_to_nume ric_type and promote is that promote may be applied to an expression of any expression type, with an attempt to promote to any expression type. However, if an expression has a non-numeric type, it can only be “promoted” to the type it already has; promoting to any other type is not possible.
