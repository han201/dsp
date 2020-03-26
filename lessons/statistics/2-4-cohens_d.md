[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

m1 = firsts.totalwgt_lb.mean() '\n'
m2 = others.totalwgt_lb.mean()
var1 = firsts.totalwgt_lb.var()
var2 = others.totalwgt_lb.var()
n1, n2 = len(firsts), len(others)
pooled_var = (n1*var1 + n2*var2) / (n1 + n2)
d = (m1-m2) / math.sqrt(pooled_var)
-0.08867292707260174
p1 = firsts.prglngth.mean()
p2 = others.prglngth.mean()
v1 = firsts.prglngth.var()
v2 = others.prglngth.var()
pooled_v = (n1*v1 + n2*v2) / (n1 + n2)
dd = (p1-p2) / math.sqrt(pooled_v)
0.028879044654449834

# First babies are indeed lighter and take longer pregnancy length
