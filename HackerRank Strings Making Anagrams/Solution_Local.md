package main;

import java.util.ArrayList;
import java.util.HashMap;
import java.util.Map;

public class String_Making_Anagrams {


	public static Map<String, Integer> myStri(String a)    {

		Map<String, Integer>  map= new HashMap<>();

		for(int i=0;i<a.length();i++)
		{
			if(map.containsKey(String.valueOf(a.charAt(i)))) 
			{
				int val = map.get(String.valueOf(a.charAt(i)));
				val+=1;
				map.put(String.valueOf(a.charAt(i)), val);
			}
			else {
				map.put(String.valueOf(a.charAt(i)),1); 	
			}
		}
		return map;
	}


	static int makeAnagram(String a, String b) {
		int deletions = 0;

		Map<String, Integer>  map1= new HashMap<>();
		Map<String, Integer>  map2= new HashMap<>();

		map1 = myStri(a);
		map2 = myStri(b);

		for(String x:map1.keySet())
		{
			if(map2.containsKey(x))
			{
				deletions += Math.abs(map2.get(x)-map1.get(x));

			} else {
				deletions += map1.get(x);
			}
		}

		for(String x:map2.keySet())
		{
			if(!map1.containsKey(x))
			{
				deletions += map2.get(x);
			}
		}

		return deletions;
	}

	public static void main(String[] args) {
		String a = "abcd";
		String b = "abcdaae";
		Map<String, Integer>  map1= new HashMap<>();
		Map<String, Integer>  map2= new HashMap<>();

		map1 = myStri(a);
		map2 = myStri(b);

		System.out.println(map1);
		System.out.println(map2);
		
		int del = 0;
		del= makeAnagram(a,b);
		System.out.println(del);
	}

	//	public static ArrayList<String> myStr(String a)    {
	//
	//		ArrayList<String> stringlist = new ArrayList<>();
	//
	//		for(int i=0;i<a.length();i++)
	//		{
	//			stringlist.add(i,String.valueOf(a.charAt(i))); 	
	//		}
	//		return stringlist;
	//	}


}
