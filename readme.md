Example of object builder for inherited objects that add new methods.

*Example:*
```
class a { void ma(s); }
class b extends a { void mb(s); }
class c extends b { void mc(s); }
class d extends c { void md(s); }

A a = A.newBuilder().ma("a").build();
B b = B.newBuilder().ma("a").mb("b").build();
C c = C.newBuilder().ma("a").mb("b").mc("c").build();
D d = D.newBuilder().mb("b").ma("b").mc("c").md("d").build();
```
