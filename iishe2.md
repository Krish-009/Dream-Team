- **NetID:** iishe2
- **Major:** Computer Science
- **Question that I chose from the memoization exercise:** climbing the stairs
- **Link to the question article:** https://www.geeksforgeeks.org/dsa/count-ways-reach-nth-stair/

- **My solution:**
class Solution {
  public:
    int nthStair(int n) {
        //  Code here
        int numOfWays = 0;
        if(n == 0){
            return 1;
        }
        numOfWays += nthStair(n - 1);
        numOfWays += nthStair(n - 2);
        return numOfWays;
    }
};
