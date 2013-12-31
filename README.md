cc.vicp.iisure
==============
Only need three steps, you can parse an xml
1.The first step in creating a bean example
pubilc class Person{
    private String name;
    private String age;
    
    public setName(String Name){
          .......
    }
    
    public getName(){
          .....
    }
    .....
}

2.The second step, create XmlPullParseUtil

 XmlPullParse = new XmlPullParseUtil(new FileInputStream(/,,) or from the web getInputStream);

3.The The third step,call parseXML method

XmlPullParse.parseXML(new Person())

Only need three steps, Serialized bean to xml
1.The first step in creating a bean example  and the bean is instantiated into the list after collection
pubilc class Person{
    private String name;
    private String age;
    
    public setName(String Name){
          .......
    }
    
    public getName(){
          .....
    }
    .....
}

List<Person> list = new ArrayList<Person>();
list.add(new Person());

2.The second step, create XmlSerializerUtil

 XmlSerializer = new XmlSerializerUtil(new FileOutputStream(/,,));

3.The The third step,call SerializedXml method

XmlSerializer.SerializedXml(list)
