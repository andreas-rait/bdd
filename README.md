bdd_lesson
==========

bdd fh lesson

---Simple Text Munger----

Feature: Simple Text Munger
In order to munge some words
As a user 
I want the SimpleTextMunger to munge some words for me


-------------------------------------------------------

CucumberOptions:

features = "[yourpath]/SimpleTextMunger.feature", format = {"pretty", "html:target/cucumber"}
yourpath e.g: src/test/resources/at/fhjoanneum/aim/bdd_lesson


----------------------------------------------------------


Spring:

src/test/resources/cucumber.xml:

<?xml version="1.0" encoding="UTF-8"?>
<beans
    xmlns="http://www.springframework.org/schema/beans"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns:context="http://www.springframework.org/schema/context"
    xsi:schemaLocation=
    "http://www.springframework.org/schema/beans
     http://www.springframework.org/schema/beans/spring-beans-3.0.xsd
     http://www.springframework.org/schema/context
     http://www.springframework.org/schema/context/spring-context-3.0.xsd">

    <context:component-scan base-package="at.fhjoanneum.aim.bdd_lesson"/>
    <context:annotation-config/>
    <import resource="classpath*:/applicationContext.xml"/>
</beans>


src/test/resources/spring/applicationContext.xml

<?xml version="1.0" encoding="UTF-8"?>
<beans
    xmlns="http://www.springframework.org/schema/beans"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns:context="http://www.springframework.org/schema/context"
    xsi:schemaLocation=
    "http://www.springframework.org/schema/beans
     http://www.springframework.org/schema/beans/spring-beans-3.0.xsd
     http://www.springframework.org/schema/context
     http://www.springframework.org/schema/context/spring-context-3.0.xsd">

    <context:component-scan base-package="at.fhjoanneum.aim.bdd_lesson"/>
</beans>


-------------------------------------------------

