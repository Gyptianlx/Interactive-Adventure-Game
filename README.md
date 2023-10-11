My Interactive Adventure Game (unfinished)

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
			std::this_thread::sleep_for(std::chrono::milliseconds(60));
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
			type_text(" This game is about focus and sheer I M B E C I L I T Y \n");
			type_text("            Have fun my fellow traveller!               \n");
			type_text("                                                     \n \n");
			type_text("        ++ - - - - L O O O O A D I N G - - - - ++    \n \n");

			type_text("                          Dun!                    \n \n \n");

			std::cout << "Enter your character's name: ";
			std::cin >> c_name;
			std::cout << " Hello " << c_name << "." " Welcome to Adventure Island. ";
			type_text(" I see you have come prepared for combat. I'm glad you came along, we haven't had a volunteer sacrifice in years \n");
			std::cout << "c_name " << "Years??? ";
			std::cout << " You're a warrior " << c_name << "." << "You fear nothing. \n \n";
			type_text(" Here we are. The valley of Man Eating Flowers. \n");
			type_text(" Our people are in danger. There is an evil and treacherous band of gorillas on the island \n");
			type_text(" They have been holding us captive for generations and have stolen our Sacred Banana \n");
			type_text(" We Need your help to go to Machuchu Mountain and take back our \n");
			type_text(" Sacred Banana from the evil gorillas. You are our only hope! \n \n");
			std::cout << "Will you help us" << c_name << "? ";
			std::cout << "Y / N";
			std::cin >> decision;

			if (decision == 'y') {
				std::cout << " Wonderful news " << c_name << "." << " I will alert my monkey people of your bravery at once!";
				std::cout << " You are much appreciated " << c_name << ".";
				type_text(" GOOD LUCK! \n \n ");
			}
			std::cout << "Start travelling? ";
			std::cin >> decision;

			if (decision == 'y') {
				std::cout << " You venture into the Valley of Man Eating Flowers. ";
			}
			else if (decision == 'n') {
				std::cout << "Your character is waiting for you to start.";
			}


			type_text(" The sun shines from beyond moving the grey clouds. \n ");
			type_text(" The bushes rustle as the wind pushes them violently. \n ");
			type_text(" You keep walking along the dense forest, seeing the faint sunlight climb down between the tree leaves, until you come to a shallow stream \n ");
			type_text(" As you get closer to the stream, the wind slows, the bushes get silent . . .                                               \n ");
			type_text(" The birds stop chirping and the frogs hide.                                                                                \n ");
			type_text(" You look around for the sound of brambles snapping all around.                                           \n \n");
			std::cout << "Will you stay and find out? ";
			std::cin >> decision;

			if (decision == 'y') {
				std::cout << " You will now be comsumed by the carnivorous vines wrapping tightly around your feet. ";
			}
			else if (decision == 'n') {
				std::cout << " You swim accross the stream to safety? ";
			}
			std::cout << "Cry for help? ";
			std::cin >> decision;



			if (decision == 'y') {
				std::cout << " You're wasting your time. No one is coming to help ";

			}
			else if (decision == 'n') {
				std::cout << " You have faught foolishly, worthy of recognition in the Council of Ediocracy ";
			}

			type_text(" You watch as the hungry vines show themselves accross the stream, hungrily waiting. \n");
			type_text(" Your heart pounding for what could have been the end \n");


		
		std::cout << "Do you want to play again? ";
		std::cout << "Y / N";
		std::cin >> start_over;
	}while (start_over == 'y' || start_over == 'Y');
		std::cout << "Thank you for playing!";
		type_text(" Hope you enjoyed :) ");
		return 0;
	
}
