package main; <br>

import java.util.ArrayList; <br>
import java.util.HashMap; <br>
import java.util.Map; <br>

public class String_Making_Anagrams { <br>


	public static Map<String, Integer> myStri(String a)    { <br>

		Map<String, Integer>  map= new HashMap<>(); <br>

		for(int i=0;i<a.length();i++) <br>
		{ <br>
			if(map.containsKey(String.valueOf(a.charAt(i))))  <br>
			{ <br>
				int val = map.get(String.valueOf(a.charAt(i))); <br>
				val+=1; <br>
				map.put(String.valueOf(a.charAt(i)), val); <br>
			} <br>
			else { <br>
				map.put(String.valueOf(a.charAt(i)),1); 	<br>
			} <br>
		} <br>
		return map; <br>
	} <br>


	static int makeAnagram(String a, String b) { <br>
		int deletions = 0; <br>

		Map<String, Integer>  map1= new HashMap<>(); <br>
		Map<String, Integer>  map2= new HashMap<>(); <br>

		map1 = myStri(a); <br>
		map2 = myStri(b); <br>

		for(String x:map1.keySet()) <br>
		{ <br>
			if(map2.containsKey(x)) <br>
			{ <br>
				deletions += Math.abs(map2.get(x)-map1.get(x)); <br>

			} else { <br>
				deletions += map1.get(x); <br>
			} <br>
		} <br>

		for(String x:map2.keySet()) <br>
		{ <br>
			if(!map1.containsKey(x)) <br>
			{ <br>
				deletions += map2.get(x); <br>
			} <br>
		} <br>

		return deletions; <br>
	} <br>

	public static void main(String[] args) { <br>
		String a = "abcd"; <br>
		String b = "abcdaae"; <br>
		Map<String, Integer>  map1= new HashMap<>(); <br>
		Map<String, Integer>  map2= new HashMap<>(); <br>

		map1 = myStri(a); <br>
		map2 = myStri(b); <br>

		System.out.println(map1); <br>
		System.out.println(map2); <br>
		
		int del = 0; <br>
		del= makeAnagram(a,b); <br>
		System.out.println(del); <br>
	} <br>

	//	public static ArrayList<String> myStr(String a)    { <br>
	// <br>
	//		ArrayList<String> stringlist = new ArrayList<>(); <br>
	//<br>
	//		for(int i=0;i<a.length();i++) <br>
	//		{ <br>
	//			stringlist.add(i,String.valueOf(a.charAt(i))); 	<br>
	//		} <br>
	//		return stringlist; <br>
	//	} <br>


} <br>
