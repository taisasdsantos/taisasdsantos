class Pessoa():
    def _init_(self, nomeAluno, pesoAluno, idadeAluno, comendo=False, falando=False, dormindo=False):
        self.nome = nomeAluno
        self.peso = pesoAluno
        self.idade = idadeAluno
        self.comendo = comendo
        self.falando = falando
        self.dormindo = dormindo

    def comer(self, alimento):
        if self.comendo == False and self.falando == False and self.dormindo == False and self.comendo == False:
            self.comendo = True
            print(f"{self.nome} começou a comer.")
        else:
            if self.comendo == True:
                print(f"{self.nome} não pode pois ele já esta comendo.")
            elif self.dormindo == True:
                print(f"{self.nome} não pode pois ele está dormindo.")
            elif self.falando == True:
                print(f"{self.nome} não pode pois ele ja está falando.")

    def parardecomer(self):
        if self.comendo == True:
            self.comendo = False
            print(f"{self.nome} parou de comer.")
        else:
            if self.dormindo == True:
                print(f"{self.nome} não pode pois ele está dormindo.")
            elif self.falando == True:
                print(f"{self.nome} não pode pois ele já esta falando.")
            elif self.comendo == False:
                print(f"{self.nome} não pode pois ele ja está comendo.")
                

    def falar(self):
        if self.falando == False and self.falando == False and self.dormindo == False and self.comendo == False:
            self.falando = True
            print(f"{self.nome} começou a falar .")
        else:
            if self.dormindo == True:
                print(f"{self.nome} não pode pois ele está dormindo.")
            elif self.comendo == True:
                print(f"{self.nome} não pode pois ele ja está comendo.")
            elif self.falando == True:
                print(f"{self.nome} não pode pois ele já esta comendo.")
                
    def paroudefalar(self):
        if self.falando == True:
            print(f"{self.nome} parou de falar.")
            self.falando = False
        else: 
            if self.comendo == True:
                print(f"{self.nome} não pode pois ele ja está comendo.")
            if self.dormindo == True:
                print(f"{self.nome} não pode pois ele ja está dormindo.")
            

    def acordou(self):
        if self.dormindo == True:
         print(f"{self.nome} acordou.")
         self.dormindo = False 
        else:
            if self.falando == True:
                print(f"{self.nome} não pode pois ele já esta falando.")
            elif self.dormindo == True:
                print(f"{self.nome} não pode pois ele está dormindo.")
            elif self.comendo == True:
                print(f"{self.nome} não pode pois ele ja está comendo.")
        
    def dormir(self):
        if self.dormindo == False:
            self.dormindo = True
            print(f"{self.nome} começou a dormir.")
        else:
            if self.falando == True:
                print(f"{self.nome} não pode pois ele já esta falando.")
            elif self.dormindo == True:
                print(f"{self.nome} não pode pois ele está dormindo.")
            elif self.comendo == True:
                print(f"{self.nome} não pode pois ele ja está comendo.")
