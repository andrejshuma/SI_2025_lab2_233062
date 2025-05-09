Andrej Shumanovski 233062

2. CFG image 

3.Ciklomatska kompleksnost mozeme da presmetame kako C = P + 1

vo nashiot kod p (brojot na predicate nodes) e 7. zatoa C = 7 + 1
C = 8


4. Potrebni se 5 test cases za da se opfatat site statements. Prviot test case e za listata so vrednost null za da dobieme exeption
vtoriot test case e item bez ime za da dobieme exeption
tretiot test case e skap item za da dodademe popust
cetvrtio test case e nevaliden cardnum za da vidime exept
i pettiot test case e prazna lista od items i validna karticka

Statement	allItems = null, cardNumber = "123"	 | allitems=[("",100,0,1)], cardNumber=1234567891234567 | 	allitems=[("exp",350,0,1)], cardNumber=1234567891234567 |	allitems=[("ime",100,0,1)], cardNumber=123	| allitems=[], cardNumber=1234567891234567
1	✓	✓	✓	✓	✓
2	✓				
3		✓	✓	✓	✓
4		✓	✓	✓	✓
5		✓	✓	✓
6		✓	✓	✓
7		✓			
8			✓	✓
9			✓		
10			✓	✓
11					
12			✓	✓
13			✓	✓	✓
14			✓		✓
15			✓		✓
16			✓		✓
17			✓		✓
18			✓		✓
19					
20				✓
21			✓		✓ 

5. Za ovoj kriterium ni trebaat 4 sluchaevi bidejkji treba da gi opfatime samo TXX XTX XXT FFF

if (item.getPrice() > 300 || item.getDiscount() > 0 || item.getQuantity() > 10).
TXX	item=Item(350,0,0)
XTX	item=Item(350,10,0)
XXT	item=Item(350,0,120)
FFF	item=Item(250,-10,-10)