def caesar_cipher(str, shift)
    alphabet = Array('a'..'z')
    non_caps = Hash[alphabet.zip(alphabet.rotate(shift))]
    
    alphabet = Array('A'..'Z')
    caps = Hash[alphabet.zip(alphabet.rotate(shift))]
    
    encryped_word = str.chars.map do |c|
      if non_caps.include?(c)
        non_caps[c]
      elsif caps.include?(c)
        caps[c]
      else
        c
      end
    end
    
    return encryped_word.join
  end
  
  puts caesar_cipher("I am Jack!", 4)
 