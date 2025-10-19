# Template-Method
```cs
abstract class AbstractClass {
    public void TemplateMethod(){
        Step1(); Step2();
    }
    protected abstract void Step1();
    protected abstract void Step2();
}

class ConcreteClass : AbstractClass {
    protected override void Step1()=>Console.WriteLine("Step1");
    protected override void Step2()=>Console.WriteLine("Step2");
}

class Program { static void Main()=>new ConcreteClass().TemplateMethod(); }
