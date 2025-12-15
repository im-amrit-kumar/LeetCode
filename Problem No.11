class Solution {
    public int maxArea(int[] height) {
        if (height == null || height.length < 2) return 0;
        int left = 0, right = height.length - 1;
        int max = 0;
        while (left < right) {
            int hl = height[left], hr = height[right];
            int area = (hl < hr ? hl : hr) * (right - left);
            if (area > max) max = area;
            if (hl < hr) left++;
            else if (hl > hr) right--;
            else { left++; right--; } 
        }
        return max;
    }
}
