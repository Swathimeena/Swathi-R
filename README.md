# Swathi-R
from datetime import date
class student:
   
    def _init_(self,name,gender,city,dob):
        self.name = name
        self.gender = gender
        self.city = city
        self.dob = dob
        
    @classmethod
    def stu_data(cls,data):
    	name,gender,city,dob=data.split(",")
    	return cls(name,gender,city,dob)
    @staticmethod
    def job(year):
    	avaiable_year=[2000,2002]
    	if year in avaiable_year:
    		return True
    	return   False
   	
   
stu1 = student("suresh","Male","bangalore",1999)
stu2 = student("malar","Female","trichy",2001)

data='Swathi,female, Krishnagiri,2003'
stu3=student.stu_data(data)
print(stu3.name)
print(stu3.gender)
print(stu3.city)
print(stu3.dob)
print(stu1.job(1999))
print(stu2.job(2001))
