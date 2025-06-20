# emojis-responder-1-project
# Emoji-Mood-Responder
import java.util.HashMap;
import java.util.Scanner;

public class EmojiMoodResponder {
    public static void main(String[] args) {
       
        
       
        moodResponses.put("happy", "😊 - Keep spreading that joy wherever you go!");
        moodResponses.put("sad", "😢 - Remember, every storm eventually passes. You've got this!");
        moodResponses.put("tired", "😴 - Rest is not a luxury, it's a necessity. Take a break!");
        moodResponses.put("excited", "🤩 - That enthusiasm is contagious! Channel it into something great!");
        moodResponses.put("angry", "😠 - Take a deep breath. You're stronger than whatever is bothering you.");
        moodResponses.put("confused", "😕 - It's okay not to have all the answers. Take it one step at a time.");
        moodResponses.put("love", "❤️ - The world needs more of what you're feeling!");
        moodResponses.put("sick", "🤒 - Your health comes first. Take care and get well soon!");
        moodResponses.put("bored", "🥱 - Adventure is out there! Try something new today.");
        moodResponses.put("surprised", "😲 - Life's full of unexpected moments. Enjoy this one!");
        moodResponses.put("silly", "🤪 - Never lose that playful spirit. It keeps life fun!");
        moodResponses.put("anxious", "😰 - Focus on your breathing. This moment will pass.");
        moodResponses.put("confident", "💪 - That self-assurance looks good on you!");
        moodResponses.put("grateful", "🙏 - Gratitude turns what we have into enough.");
        
       
        
        String userMood = scanner.nextLine().toLowerCase().trim();
        
        
        if (moodResponses.containsKey(userMood)) {
            System.out.println("\n" + moodResponses.get(userMood));
        } 
     
        else {
            System.out.println("\nHmm, I'm not familiar with that mood. Here are some I know:");
            for (String mood : moodResponses.keySet()) {
                System.out.print(mood + " ");
            }
            System.out.println("\n\nTry one of these next time!");
        }
        
        scanner.close();
    }
}
