# 2018-class-test
2018校招真题
题目链接：https://www.nowcoder.com/practice/58b04ed2865f4ff4921290f1bd4ee486?tpId=90&tqId=30811&rp=2&ru=%2Fta%2F2018test&qru=%2Fta%2F2018test%2Fquestion-ranking&tPage=2
Java版：
import java.util.Scanner;

public class ThroughRoom {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int n = input.nextInt();
        int mod = 1000000007;
        int door = input.nextInt();
        int result[] = new int[n + 1];
        for (int i = 2; i < n + 1; i++) {
            result[i] = ((result[i - 1] * 2) % mod - result[door] + 2) % mod;
            door = input.nextInt();
        }

        System.out.println(((result[n] * 2) % mod - result[door] + 2) % mod);
    }
}


Python版：
n = int(input())
p = list(map(int,input().split()))
mod = 1000000007
dp = [0]
for i in range(1,n + 1):
    dp.append(0)
    dp[i] = (2 * dp[i - 1] - dp[p[i - 1] - 1] + 2)% mod
print(dp[n])
