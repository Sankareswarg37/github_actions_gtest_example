class C{};
class B{
    C* ptr;
    public:
    B(C* addressOfObject): ptr(addressOfObject){

    }
};


class A{
    B* ptr;
    public:
    A(B* addressOfObject): ptr(addressOfObject){

    }
    bool operation(){
        return true;
    }
};

TEST("TestFixtureTestSuite", "OperationTrueTest"){
    //Arrange
    C cobj;
    B bobj(&cobj);
    A obj;

    //Act and Assert
    ASSERT_TRUE(obj.operation());
}

TEST("TestFixtureTestSuite", "OperationFalseTest"){
    //Arrange
    C cobj;
    B bobj(&cobj);
    A obj;

    //Act and Assert
    ASSERT_FALSE(obj.operation());
}