# dependabot-bug

Minimal reproduction of dependabot bug I encountered where adding cooldown makes docker updates fail.

Here dockerfile has alpine:3.20.0 defined which is over 1 year old. If cooldown is defined dependabot doesn't try to update it. How ever when cooldown is removed it gets updated as it should. With private registry cooldown causes different type of errors.
