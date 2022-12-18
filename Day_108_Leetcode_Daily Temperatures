class Solution {
    public int[] dailyTemperatures(int[] temperatures) {
        int[] ret = new int[temperatures.length];
        if(temperatures.length == 0) return ret;
        
        Stack<Integer> st = new Stack<>();
        for(int i = 0;i < temperatures.length;++i) {
            while(!st.empty() && temperatures[i] > temperatures[st.peek()]) {
                int index = st.pop();
                ret[index] = i - index;
            }
            st.push(i);
        }
        while(!st.empty()) {
            ret[st.pop()] = 0;
        }
        return ret; 
    }
}
