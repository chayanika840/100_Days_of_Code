class Solution {
    public long findTheArrayConcVal(int[] nums) {
        
        long res = 0;
        int i = 0;
        int j= nums.length-1;
        
        while(i<j){
            int num = concatenate(nums[i++],nums[j--]);
            res += num;
        }
        if((nums.length&1) != 0){
            res += nums[i];
        }
        return res;
    }
    private int concatenate(int x,int y){
        return Integer.parseInt(String.valueOf(x)+String.valueOf(y));
    }
}
