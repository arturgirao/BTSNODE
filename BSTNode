 class BSTNode(object):
    def __init__(self, key, value = None, left = None, right = None, parent = None):
        self.key = key
        self.value = value
        self.left = left
        self.right = right
		self.parent = parent
		
		def hasLeftChild(self):
		  return self.left is not None
		  
		def hasRightChild(self):
		  return self.right is not None
		
		def add(self, node):
			if node.key < self.key:
				if self.left is None:
					self.left = node
					node.parent = self
				else:
					self.left.add(node)
			if node.key >= self.key:
				if self.rigth is None:
					self.right = node
					node.parent = self
				else:
					self.right.add(node)

    def search(self, key):
        if key == self.key:
            return self
        if key < self.key and self.left:
            return self.left.search(key)
        if key > self.key and self.right:
            return self.right.search(key)

    def in_order(self):
        if self.left:
            self.left.in_order()
        print(self.key)
        if self.right:
            self.right.in_order()

    def pre_order(self):
        print self.key
        if self.left:
            self.left.pre_order()
        if self.right:
            self.right.pre_order()

    def pos_order(self):
        if self.left:
            self.left.pos_order()
        if self.right:
            self.right.pos_order()
        print self.key


   def find_minimun(self):
	if self.left:
		return sel.left.find_minimum()
	else
		return self

   def find_maximun(self):
	if self.right:
		return self.right.find_maximum()
	else
		return self
		
		

	





root = BSTNode(10)

root.left = BSTNode(7)
root.right = BSTNode(18)

root.left.left = BSTNode(3)
root.left.right = BSTNode(9)
root.left.left.left = BSTNode(1)
root.left.right.left = BSTNode(8)

root.right.left = BSTNode(11)

minimun = root.find_minimum()
maximun = root.find_maximun()

print("===== Minimo ====")
print (minimun.key)

print("===== Máximo ====")
print (maximun.key)

print("===== Executando in-order =====")
root.in_order()

print("===== Executando pre-order =====")
root.pre_order()

print("===== Executando pos-order =====")
root.pos_order()


