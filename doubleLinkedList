class Node:
def __init__(self, data):
self.data = data
self.next = None
self.prev = None
class DoubleLinkedList:
def __init__(self):
self.head = None
self.tail = None

def add__front(self, new):
if self.head is None:
self.head = new
self.tail = new
else:
new.next = self.head
self.head.prev = new
self.head = new
def add__tail(self, new):
if self.tail is None:
self.tail = new
self.head= new
else:
self.tail.next = new
new.prev = self.tail
self.tail = new
def add__between(self, new, search):
temp = self.head
if self.head is None:
self.head = new
self.tail = new
else:
while temp is not search:
temp = temp.next
new.next = temp.next
new.prev = temp
temp.next = new
temp.next.next.prev = new
def traverse__head(self):
temp = self.head
while temp is not None:
print(temp.data)
temp = temp.next
def traverse__tail(self):
temp = self.tail
while temp is not None:
print(temp.data)
temp = temp.prev
#sametgumus1@aydin.edu.tr
aa = Node("3")
aa1 = Node("5")
aa2 = Node("6")
aa3 = Node("7")
aa4 = Node("9")

bb = DoubleLinkedList()
bb.add__tail(aa)
bb.add__tail(aa1)
bb.add__tail(aa2)
bb.add__tail(aa3)
bb.add__between(aa4, aa2)


bb.traverse__head()
bb.traverse__tail()
