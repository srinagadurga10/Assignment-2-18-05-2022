# Assignment-2-18-05-2022
Assignment 2
def subarraysDivByK(self, num: List[int], k: int) -> int: c=0 sums=0 d={} d[0]=1 for i in num: c+=i c%=k if c<0: c+=k if c in d: sums+=d[c] else: d[c]=0 d[c]+=1 return sums

