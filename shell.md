# shell python + Django

# instale o ipython
    pip install ipython    

## rodando o shell python  
    ./manager.py shell

##  importando model
    from modulo.models import NomeDaClasse

##  salvando  
    todo = Todo()
    todo.name = "Gleison de souza luiz"
    todo.save()

## visualizar dados cadastrados
    todo.__dict__    

# serializando via shell


### importando o necessário 
    from app.models import Todo
    from app.serializer import TodoSerializer

### instanciando primeiro objeto 
    todo = Todo.objects.first()
### serializando
    serializer = TodoSerializer(todo)
### exibindo objeto data do serializer
    serializer.data    