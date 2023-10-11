# Interactive-Adventure-Game
Interactive Adventure Game

#include <iostream>
#include <thread> // standard C++11


	// function to output as if it was being typed
	void type_text(const std::string & text)
	{
		// loop through each character in the text
		for (std::size_t i = 0; i < text.size(); ++i)
		{
			// output one character
			// flush to make sure the output is not delayed
			std::cout << text[i] << std::flush;

			// sleep 60 milliseconds
			std::this_thread::sleep_for(std::chrono::milliseconds(20));
		}
	}
	int main()

	{
		char decision;
		char start_over;
		do {
			std::string c_name;
			char decision;

			type_text("             Welcome to Adventure Island                \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(400));

			type_text("     This game is about focus and sheer foolishness     \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(1800));

			type_text("            Have fun my fellow traveller!               \n");
			type_text("                                                     \n \n");
			type_text(" ++ - - Loading - the - Beetles - and - Bugs - - ++  \n \n");

			type_text("                          Dun!                    \n \n \n");

			std::cout << "Enter your character's name: \n";
			std::cin >> c_name;
			std::cout << " Hello " << c_name << ". Welcome to Adventure Island. \n";
			type_text(" I see you have come prepared for combat. \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(1000));

			type_text(" I'm glad you came along, we haven't had a volunteer sacrifice in years.. \n \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(1500));

			std::cout << " You're a warrior " << c_name << ". \n";

			std::this_thread::sleep_for(std::chrono::milliseconds(1000));

			type_text(" You fear nothing! \n \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(1000));

			type_text(" We must travel at once! \n \n \n \n ");

			std::this_thread::sleep_for(std::chrono::milliseconds(3000));

			type_text(" Preparing beetles [OK] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(50));
			type_text(" Looking for centipeas [OK] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(35));
			type_text(" Putting rocks back [OK] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(40));
			type_text(" Climbing trees [OK] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(40));
			type_text(" Stealing Berries [OK] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(60));
			type_text(" chasing birds [OK] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(20));
			type_text(" admiring skies [OK] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(30));
			type_text(" climbing hills [OK] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(90));
			type_text(" Evading mosquitoes [Bitten] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(30));
			type_text(" Wiggling through water [OK] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(25));
			type_text(" Drying feathers. [OK] \n ");
			std::this_thread::sleep_for(std::chrono::milliseconds(200));
			type_text(" Dun! \n \n ");

			type_text(" - + - Terrain Loaded - + - \n \n \n ");


			type_text(" Here we are, Chama Chu Chu. \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(2000));

			type_text(" The valley of Man Eating Forest. \n \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(2000));

			type_text(" Our people are in danger! \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(1000));

			type_text(" There is an evil and treacherous band of gorillas on the island. \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(1000));

			type_text(" They have been holding us captive for generations and have stolen our Sacred Banana. \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(2500));

			type_text(" We Need your help to go to Machuchu Mountain and take back our Sacred Banana from the evil gorillas. \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(1000));

			type_text(" You are our only hope! \n \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(2000));


			std::cout << "Will you help us " << c_name << "? (Y / N) ";
			std::cin >> decision;

			if (decision == 'y') {
				std::cout << " Wonderful news " << c_name << ". \n";

				std::this_thread::sleep_for(std::chrono::milliseconds(750));

				std::cout << " I will alert my monkey people of your bravery at once! \n";

				std::this_thread::sleep_for(std::chrono::milliseconds(1500));

				std::cout << " You are much appreciated " << c_name << ". \n";

				std::this_thread::sleep_for(std::chrono::milliseconds(1000));

				type_text(" GOOD LUCK! \n \n ");
			}
			else if (decision == 'n') {
				std::cout << "You rejected Yellow Monkeys' offer. :( ";

				std::cout << "Do you want to play again? ";
				std::cout << "Y / N";
				std::cin >> start_over;
				while (start_over == 'y' || start_over == 'Y');
				std::cout << "Thank you for playing!";

				std::this_thread::sleep_for(std::chrono::milliseconds(1000));

				type_text(" Hope you enjoyed :) ");
				return 0;
			}

			std::cout << " You venture into the Valley of Man Eating Forest. \n ";

			std::this_thread::sleep_for(std::chrono::milliseconds(1500));

			type_text(" The sun shines from beyond moving the grey clouds. \n ");

			std::this_thread::sleep_for(std::chrono::milliseconds(1000));

			type_text(" The bushes rustle as the wind pushes them violently. \n ");

			std::this_thread::sleep_for(std::chrono::milliseconds(1000));

			type_text(" You keep walking along the dense forest, seeing the faint sunlight climb down between the tree leaves, until you come to a shallow stream \n ");

			std::this_thread::sleep_for(std::chrono::milliseconds(4000));

			type_text(" As you get closer to the stream, the wind slows, the bushes get silent . . . \n ");

			std::this_thread::sleep_for(std::chrono::milliseconds(750));

			type_text(" The birds stop chirping and the frogs hide. \n ");

			std::this_thread::sleep_for(std::chrono::milliseconds(1200));

			type_text(" You look around for the sound of brambles snapping all around. \n \n");

			std::this_thread::sleep_for(std::chrono::milliseconds(2000));

			std::cout << "Will you stay and find out? ";
			std::cin >> decision;

			if (decision == 'y') {
				std::cout << " You will now be comsumed by the carnivorous vines wrapping tightly around your feet. ";
			}
			else if (decision == 'n') {
				std::cout << " You swim accross the stream to safety? ";

				std::this_thread::sleep_for(std::chrono::milliseconds(3500));

			}
			std::cout << "Cry for help? ";
			std::cin >> decision;



			if (decision == 'y') {
				std::cout << " You're wasting your time. No one is coming to help ";

				std::this_thread::sleep_for(std::chrono::milliseconds(1000));
				std::cout << "Do you want to play again? ";
				std::cout << "Y / N";
				std::cin >> start_over;
				while (start_over == 'y' || start_over == 'Y');
				std::cout << "Thank you for playing!";

				std::this_thread::sleep_for(std::chrono::milliseconds(1000));

				type_text(" Hope you enjoyed :) ");
				return 0;

			}
			else if (decision == 'n') {
				std::cout << " You have faught foolishly, worthy of recognition in the Council of Ediocracy ";

				std::this_thread::sleep_for(std::chrono::milliseconds(1000));

				std::cout << "Do you want to play again? ";
				std::cout << "Y / N";
				std::cin >> start_over;
				while (start_over == 'y' || start_over == 'Y');
				std::cout << "Thank you for playing!";

				std::this_thread::sleep_for(std::chrono::milliseconds(1000));

				type_text(" Hope you enjoyed :) ");
				return 0;
			}

			std::this_thread::sleep_for(std::chrono::milliseconds(3000));
			std::cout << c_name << " swims accross the stream to safety? ";
			type_text(" You watch as the hungry vines show themselves accross the stream, hungrily waiting. \n");
			type_text(" Your heart pounding for what could have been the end.. \n");



			std::cout << "Do you want to play again? ";
			std::cout << "Y / N";
			std::cin >> start_over;
		} while (start_over == 'y' || start_over == 'Y');
		std::cout << "Thank you for playing!";
		type_text(" Hope you enjoyed :) ");

		return 0;
	
}
