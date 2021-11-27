# Richest-Customer-Wealth
#Array Leetcode Problem Solution
class Solution {
    public int maximumWealth(int[][] accounts) {
        int r=accounts.length;
        int c=accounts[0].length;
        int sum1;
        int max=0;
        for(int i=0;i<r;i++)
        {
            sum1=0;
            for(int j=0;j<c;j++)
            {
                sum1=sum1+accounts[i][j];
            }
            if(max<sum1)
            {
                max=sum1;
            }
        }
        return max;
    }
}
