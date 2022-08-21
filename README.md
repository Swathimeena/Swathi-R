#python inheritance
# Program to show that we can create instance variables inside methods  
# Class for Animal 
class Animal:  
        
    # Class Variable  
    animal = 'Dog'      
        
    # The init method or constructor  
    def __init__(self, breed):  
            
        # Instance Variable  
        self.breed = breed              
    
    # Adds an instance variable   
    def setColor(self, color):  
        self.color = color  
        
    # Retrieves instance variable      
    def getColor(self):      
        return self.color     
    
    # Driver Code  
Rodger = Animal("Bhruno")  
Rodger.setColor("Brown")  
print(Rodger.getColor())
