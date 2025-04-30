require(contributors[msg.sender] > 0, "Sorry, you are not a contributor. Try to contribute to crowd funding then try again. Thanks.");
        _;
    }

    // All Modifiers Ends here --------------------------------------------------

    // get balance
    function getBalance() public view returns (uint256) {
        return address(this).balance;
    }

    // Contribute
    function contribute() public payable isDeadlinePassed {

    }

    // Refund the money if the target is not fulfilled and deadline has passed.
    function refund() public isDeadlinePassed isContributor {

    }

    // Create Request
    function createRequest(

    }

    // vote request.
    function voteRequest(uint256 _requestNo) public isContributor {

    }

    // make payemnt only if the voters are greater than half of the contributors.
    function makePayment(uint _requestNo) public onlyOwner{



    }
}# crowdfunding.sol
