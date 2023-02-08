n,m = input().split('+')
"""n=input()
m=input()"""
class sol:
    def RomtoInt(self, s):
        x = {'I': 1, 'V': 5, 'X': 10, 'L': 50, 'C': 100, 'D': 500, 'M': 1000}
        y = 0
        for i in range(len(s)):
            if i > 0 and x[s[i]] > x[s[i - 1]]:
                y += x[s[i]] - 2 * x[s[i - 1]]
            else:
                y += x[s[i]]
        return y
x=sol().RomtoInt(n)
y=sol().RomtoInt(m)
z=x+y
def solve(num):
   res = ""
   table = [
      (1000, "M"),
      (900, "CM"),
      (500, "D"),
      (400, "CD"),
      (100, "C"),
      (90, "XC"),
      (50, "L"),
      (40, "XL"),
      (10, "X"),
      (9, "IX"),
      (5, "V"),
      (4, "IV"),
      (1, "I"),
   ]
   for cap, roman in table:
      d, m = divmod(num, cap)
      res += roman * d
      num = m

   return res


print(solve(z))
