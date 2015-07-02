# PRINTING-OUT-THE-USER-S-GUESS-
Next, implement the function getGuessedWord that takes in two parameters - a string, secretWord, and a list of letters, lettersGuessed. This function returns a string that is comprised of letters and underscores, based on what letters in lettersGuessed are in secretWord. This shouldn't be too different from isWordGuessed!


def getGuessedWord(secretWord, lettersGuessed):
    '''
    secretWord: string, the word the user is guessing
    lettersGuessed: list, what letters have been guessed so far
    returns: string, comprised of letters and underscores that represents
      what letters in secretWord have been guessed so far.
    '''
    # FILL IN YOUR CODE HERE...
    bien = ''
    mal = ''
    for char in secretWord:                 #Check if input is in secretWord
       if char in lettersGuessed:           #if True
           bien += char                     #add letter to bien  
       else:                                #if it is not
           mal = '_'                        #add '_'
       juego = bien + mal                   #Add bien and mal to a single string
    return juego                            #Get the result from bien + mal        
