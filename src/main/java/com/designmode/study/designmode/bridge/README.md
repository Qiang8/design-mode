由代码理解什么是桥接模式：
现在只有房地产公司和山寨公司，那以后我会不会增加一些其他的公司或者房地产公司会不会对业务进行细化，比如分为公寓房公司，别墅公司，
以及商业房公司等等，这种变化对我们上面的类图没有大的修改，充其量是扩展，
增加公司，要么继承Corp类，要么继承HouseCorp或ShanZhaiCorp，不用再修改原有的类了；
增加产品，继承Product类，或者继承House类，要把房子分为公寓房、别墅、商业用房等等；
都是在扩展，唯一要修改的就是Client类，也就是说Corp类和Product类都可以自由的扩展，而不会对整个应用产生太的变更，这就是桥梁模式。

使用场景：
1、如果一个系统需要在构件的抽象化角色和具体化角色之间增加更多的灵活性，避免在两个层次之间建立静态的继承联系，通过桥接模式可以使它们在抽象层建立一个关联关系。
2、对于那些不希望使用继承或因为多层次继承导致系统类的个数急剧增加的系统，桥接模式尤为适用。
3、一个类存在两个独立变化的维度，且这两个维度都需要进行扩展。