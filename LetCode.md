# Two Sum
- Inputs:
 nums = [2, 7, 11, 15], target = 9
- Output:  
[0, 1]

```
function twoSum($nums, $target)
{
    $arr = [];
    for ($i = 0; $i < count($nums); $i++) {
        for ($j = $i+1; $j < count($nums); $j++) {
            if ($target == ($nums[$i] + $nums[$j])) {
                $arr[0] = $i;
                $arr[1] = $j;
            }
        }
    }
    return $arr;
}

print_r(twoSum([3,2,4], 6));
```