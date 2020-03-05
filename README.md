<img src="https://github.com/Antonio-Cruciani/Nystrom-Low-Rank-Approximation/blob/master/img/nystrom_lowrank.png?v=3&s=200" title="Nystrom Approximation" alt="Nystrom" height=300 width=700>


# Nystrom-Low-Rank-Approximation
Nystrom Low Rank Gram Matrix Approximation in KELP


## Table of Contents 

- [Description](#Description)
- [Nystrom Method](#Nystrom-Method)
- [Kelp](#Kelp)
- [Examples](#Examples)
- [Import Kelp](#Import-Kelp)
- [License](#License)

## Description

This library allows you to use Kernel Methods for large-scale learning problems.

## Nystrom-Method

Kernel methods project data points into a high dimensional or infinite-dimensional feature space and find the optimal splitting hyperplane. In the kernel method the data is represented in a Gram Matrix. The main problem of kernel method is its high computational cost associated with kernel matrices. The cost is at least quadratic in the number of training data points, but most kernel methods include computation of matrix inversion or eigenvalue decomposition and the cost becomes cubic in the number of training data Large training sets cause large storage and computational costs. In spite of low rank decomposition methods (Cholesky decomposition) reduce this cost, they continue to require computing the kernel matrix. One of the approaches to deal with this problem is low-rank matrix approximations. The most popular examples of them are Nyström method and the random features.

The Nyström approximation can allow a significant speed-up of the computations. This speed-up is achieved by using instead of the kernel matrix its approximation of a smaller rank.


## Kelp 
KeLP (Kernel-based Learning Platform) is a Java machine learning platform providing the implementation of Kernel-based learning algorithms, as well as kernel functions over generic data representations, e.g., vectorial data or discrete structures, such as graphs, trees, and sequences.

For more informations visit :

				http://www.kelp-ml.org

			
## Import-Kelp			
Import KELP via Maven:

```xml	
	<repositories>
		<repository>
			<id>maven2-repository.java.net</id>
			<name>Java.net Repository for Maven</name>
			<url>http://download.java.net/maven/2/</url>
			<layout>default</layout>
		</repository>

		<repository>
			<id>kelp_repo_snap</id>
			<name>KeLP Snapshots Repository</name>
			<releases>
				<enabled>false</enabled>
				<updatePolicy>always</updatePolicy>
				<checksumPolicy>warn</checksumPolicy>
			</releases>
			<snapshots>
				<enabled>true</enabled>
				<updatePolicy>always</updatePolicy>
				<checksumPolicy>fail</checksumPolicy>
			</snapshots>
			<url>http://sag.art.uniroma2.it:8081/artifactory/kelp-snapshot/</url>
		</repository>
		<repository>
			<id>kelp_repo_release</id>
			<name>KeLP Stable Repository</name>
			<releases>
				<enabled>true</enabled>
				<updatePolicy>always</updatePolicy>
				<checksumPolicy>warn</checksumPolicy>
			</releases>
			<snapshots>
				<enabled>false</enabled>
				<updatePolicy>always</updatePolicy>
				<checksumPolicy>fail</checksumPolicy>
			</snapshots>
			<url>http://sag.art.uniroma2.it:8081/artifactory/kelp-release/</url>
		</repository>
	</repositories>
```
A full version ok KeLP is available on maven in the package kelp-full. It includes all the modules that compose the library. To import the 2.2.4 version of kelp-full, you can use the following Maven dependency.
```xml
		<dependency>
			<groupId>it.uniroma2.sag.kelp</groupId>
			<artifactId>kelp-full</artifactId>
			<version>2.2.4-SNAPSHOT</version>
		</dependency>
```
