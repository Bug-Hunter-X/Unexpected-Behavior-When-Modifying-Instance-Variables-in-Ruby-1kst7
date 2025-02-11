# Unexpected Behavior When Modifying Instance Variables in Ruby

This example demonstrates a common issue in Ruby where attempting to modify an instance variable from outside its class definition doesn't work as expected. The `value=` method is not defined.  This leads to the instance variable remaining unchanged, even though the assignment seems to execute without error.

To resolve this, a setter method must be explicitly defined within the class.

## How to Reproduce

1. Run `bug.rb`
2. Observe that the output shows the value remains 10, even after attempting to change it to 20.