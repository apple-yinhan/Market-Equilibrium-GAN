split total epoch into 5 parts
nums = epoch//5

when epoch < nums:
\sigma = 1, and modules for \sigma are freezed

when epoch in [nums, 2*nums] or [3*nums, 4*nums]:
modules for \mu are freezed, learn \sigma

when epoch in [2*nums, 3*nums] or [4*nums, 5*nums]:
modules for \sigma are freezed, learn \mu