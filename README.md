# majority-element-in-array
nums = list(map(int, input("Enter numbers ").split()))
n = len(nums)
x = nums[0]
c = 1
for i in range(1, n):
    if nums[i] == x:
        c += 1
    else:
        c -= 1
    if c == 0:
        x = nums[i]
        c = 1
print("Majority Elementis ", x)
