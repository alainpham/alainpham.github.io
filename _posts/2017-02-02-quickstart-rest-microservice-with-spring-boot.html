---
layout: default
title:  "Quickstart Json RESTful microservice with Spring-Boot"
date:   2017-02-03 09:00:00 +0200
published: 2017-02-02 09:00:00 +0200
comments: true
categories: development
tags: [spring-boot, quickstart, rest, json, microservice, cloudnative, development]
github: "https://github.com/alainpham/rest-service"
---

<p>In this post you will learn how to create a RESTful microservice
	from scratch using Spring-Boot, Eclipse & Maven.</p>
<!--more-->

<p>Spring boot is one of the very popular frameworks to build
	microservices. In fact it has been chosen to be the standard for JBoss
	Fuse (Fuse Integration Services 2.0) deployments on Openshift. It can
	also be used for general java application purposes. You would be
	surprised how easy it is to create standalone packages that are capable
	of running production grade services.</p>

<p>Source code for this can be found here :
<a href="https://github.com/alainpham/rest-service">https://github.com/alainpham/rest-service</a>
</p>
<p>These are the steps of this tutorial</p>

<ul>
 	<li>Create a new simple Maven project in Eclipse</li>
 	<li>Add dependencies to Spring Boot</li>
 	<li>Launch your service</li>
</ul>

<h2>Prerequisites</h2>

<p>As a prerequisite for this tutorial you will need the following
	elements:</p>

<ul>
 	<li>Java JDK</li>
 	<li>Eclipse with maven plugin</li>
 	<li>Maven</li>
</ul>



<h2>Create a simple maven project</h2>

<p>First you must create a simple maven project. For that you can use the Eclipse Wizard</p>

<a href="/assets/images/{{page.id}}/create-new-maven-project.png"> <img
	class="center-block img-responsive"
	src="/assets/images/{{page.id}}/create-new-maven-project.png" alt="create new maven project"/></a>

<p>Chose simple project to have an empty pom.xml file</p>

<a href="/assets/images/{{page.id}}/choose-simple-project.png"> <img
	class="center-block img-responsive"
	src="/assets/images/{{page.id}}/choose-simple-project.png" alt="choose simple project in eclipse"/></a>

<p>Fill in the project details</p>

<a href="/assets/images/{{page.id}}/fill-project-infos.png"> <img
	class="center-block img-responsive"
	src="/assets/images/{{page.id}}/fill-project-infos.png" alt="fill project infos"/></a>

<h2>Edit the pom.xml file</h2>

<p>Add these parent, dependencies, and plugin blocs to your pom</p>

{% highlight xml %}
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>
	<groupId>com.test</groupId>
	<artifactId>rest-service</artifactId>
	<version>0.0.1-SNAPSHOT</version>

	<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>1.5.1.RELEASE</version>
	</parent>

	<dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-test</artifactId>
			<scope>test</scope>
		</dependency>
	</dependencies>

	<build>
		<plugins>
			<plugin>
				<groupId>org.springframework.boot</groupId>
				<artifactId>spring-boot-maven-plugin</artifactId>
			</plugin>
		</plugins>
	</build>
</project>
{% endhighlight %}


<h2>Create Application class</h2>

{% highlight java %}
package com.app;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.EnableAutoConfiguration;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.context.annotation.ComponentScan;
import org.springframework.context.annotation.Configuration;



@SpringBootApplication
public class Application {

	public static void main(String[] args) {
		SpringApplication.run(Application.class, args);
	}

}
{% endhighlight %}

<h2>Create a business model</h2>
{% highlight java %}
package com.app.model;

public class Person {

	private Long id;
	private String name;


	public Long getId() {
		return id;
	}
	public void setId(Long id) {
		this.id = id;
	}
	public String getName() {
		return name;
	}
	public void setName(String name) {
		this.name = name;
	}


}
{% endhighlight %}

<h2>Create a service</h2>
{% highlight java %}
package com.app.service;

import java.util.HashMap;
import java.util.Map;

import org.springframework.web.bind.annotation.*;

import com.app.model.Person;

@RestController
@RequestMapping(value="/svc/person")
public class PersonService {

	Map<Long, Person> personMap;

	public PersonService() {
		super();
		personMap = new HashMap< Long, Person>();


		Person p1 = new Person();
		p1.setId(1l);
		p1.setName("John Doe");


		Person p2 = new Person();
		p2.setId(2l);
		p2.setName("Jane Smith");

		personMap.put(p1.getId(), p1);
		personMap.put(p2.getId(), p2);
	}


	@RequestMapping(value="/{id}",method = RequestMethod.GET)
	public Person getPerson(@PathVariable Long id){
		return personMap.get(id);
	}
}
{% endhighlight %}

<h2>Run your application</h2>

<p>Open a command prompt in the root folder of your project and run : </p>
{% highlight shell %}
mvn spring-boot:run
{% endhighlight %}

<p>You can now also build your package and run the flat jar file</p>
{% highlight shell %}
mvn package
java -jar target/rest-service-0.0.1-SNAPSHOT.jar
{% endhighlight %}

<p>Now open your browser and consume your microservice by entering the following url</p>
{% highlight shell %}
http://localhost:8080/svc/person/1
{% endhighlight %}

<a href="/assets/images/{{page.id}}/consume.png"> <img
	class="center-block img-responsive"
	src="/assets/images/{{page.id}}/consume.png" alt="test rest service by consuming"/></a>

<p>The next post will be about how to deploy such microservices packaged in Docker containers on Openshift</p>

<p>Thanks for reading !</p>
