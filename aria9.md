# Tests for ARIA9: Using aria-labelledby to concatenate a label from several text nodes

## Procedure

For inputs that use aria-labelledby:

1. Check that ids referenced in aria-labelledby are unique and match the ids of the text nodes that together provide the label
2. Check that the concatenated content of elements referenced by aria-labelledby is descriptive for the purpose or function of the element labeled

## Expected Results

#1 and #2 are true.

If this is a sufficient technique for a success criterion, failing this test procedure does not necessarily mean that the success criterion has not been satisfied in some other way, only that this technique has not been successfully implemented and can not be used to claim conformance.
