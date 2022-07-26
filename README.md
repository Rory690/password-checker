// i made a password generator hope you like it.




Console.WriteLine("would you like me to generate a password for you?");
Console.ReadLine();
string yesorno = Console.ReadLine();
if (yesorno == "yes") ;
{
    var characters = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz@#$+=_-<.?/%^&*0123456789";
    var Charsarr = new char[8];
    var random = new Random();

    for (int i = 0; i < Charsarr.Length; i++)
    {
        Charsarr[i] = characters[random.Next(characters.Length)];
    }

    var resultString = new String(Charsarr);
    Console.WriteLine("your randomly generated password is:");
    Console.WriteLine(resultString);
    Console.WriteLine("please comfirm your password by typing it here: ");
    string pass = Console.ReadLine();
    Console.ReadLine();
    if (pass == resultString) 
    {
        Console.WriteLine("your password has bean confirmed");
    }
    else
    {
        Console.WriteLine("Rong password, please try again");
        Console.ReadLine();
        if (pass == resultString)
        {
            Console.WriteLine("Your password has bean confirmed");
        }
    }
       
  
  
}
Console.WriteLine("now Please pick a username");
string userinput = Console.ReadLine();
Console.ReadLine();
Console.WriteLine("Your new username is: " + userinput);


Console.WriteLine("To confirm your username please type it here: ");
string user = Console.ReadLine();
Console.ReadLine();
if (user == userinput)
{
    Console.WriteLine("You username is now confirmed");
}
