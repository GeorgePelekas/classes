class movies():
    
    def __init__(self,userscore,criticscore,boxoffice,date,director):
        self.userscore = userscore
        self.criticscore = criticscore
        self.boxoffice = boxoffice
        self.date = date
        self.director = director

    
    def print(self):
        print("userscore: "+str(self.userscore)+" criticscore: "+str(self.criticscore)+" boxoffice: "
        +self.boxoffice+" date: "+self.date+" director: "+self.director)
    def check(self):
        if self.userscore > self.criticscore:
            print("the difference of the score is "+str(self.userscore-self.criticscore))
            return self.userscore-self.criticscore 

Spider_Man = movies(8,5,"1606000$","6/4/2007","tobey")
Smurfs = movies(6,4,"1606000$","2/4/2001","adon")
        
Shrek = movies(10,9,"696344$","6/9/2001","akis")
Spider_Man.print()
difference = Shrek.check()
print(difference)
diafora = Spider_Man.check()
diafor = Smurfs.check()
print(max(difference,diafora,diafor))
