package acsl2019;

import java.io.File;
import java.util.ArrayList;
import java.util.Scanner;

import java.io.IOException;

public class intermediate {
	public static void main(String args[]) throws IOException {

		File file = new File("C://Users//dhars/Documents//exam.txt");
		Scanner sc = new Scanner(file);
		String input = "";

		ArrayList<Integer> arr = new ArrayList<Integer>();
		sc.useDelimiter(",|\\r\n");
		while (sc.hasNextLine()) {
			System.out.println("idk");
			while (sc.hasNext()) {
				String k = sc.next();
				arr.clear();
				int space = k.indexOf(' ');
				String ink = k.substring(0, space);
				int p = Integer.parseInt(String.valueOf(k.charAt(k.length() - 1)));
				System.out.println(k);

				for (int i = 0; i < ink.length(); i++) {
					int res = Integer.parseInt(String.valueOf(ink.charAt(i)));
					arr.add(res);
				}
				int index = (arr.size() - p);

				int value = arr.get(index);

				for (int i = 0; i < index; i++) {

					arr.set(i, java.lang.Math.abs(arr.get(i) + value));

					if (arr.get(i) > 9) {

						arr.set(i, ((arr.get(i) - 10)));
					}
					System.out.println(arr.get(i));
				}

				System.out.println(value);

				for (int i = index + 1; i < arr.size(); i++) {

					arr.set(i, java.lang.Math.abs((arr.get(i) - value)));
					System.out.println(arr.get(i));
				}

			}

		}
	}
}


