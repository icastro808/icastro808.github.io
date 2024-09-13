---
layout: essay
type: essay
title: "The Art of Asking Questions"
# All dates must be YYYY-MM-DD format!
date: 2024-09-12
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
---
_"To ask the right question is already half the solution to a problem." - Carl Jung_
<img width="300px" class="rounded float-start pe-4" src="../img/question.jpg">


<br><br>Asking questions is an integral part of growing and developing not only as an individual, but also in one’s career. However, the ability to ask the right questions is a skill in its own right, and one that can greatly influence the quality and effectiveness of the answers you receive. Whether you’re seeking advice, explanations, or troubleshooting a problem, knowing how to craft a precise, thoughtful question can significantly increase your chances of getting help that is useful not only to you, but others who may follow in your footsteps. In this essay, we will delve into what distinguishes a ‘smart’ question from a ‘not so smart’ one by analyzing two different questions asked on StackOverflow, a popular forum used for programming queries. By understanding the benefits of forming and asking smart questions, you can enhance your problem solving skills and contribute more effectively to your professional community.

## What Makes a Question ‘Not So Smart’?
These ‘not so smart’ questions are typically defined as questions that exhibit the following:
  - Lack of clear and concise wording
  - Insufficient context
  - Lack of thorough testing
  - Minimal prior research
  - Unclear expectations

To illustrate these issues, let’s examine a question from StackOverflow, poorly titled ‘_why this code not work? can you help me?_’ The user has presented three sections of their PHP code, seeking assistance in understanding why their code does not function correctly.
```
why this code not work?

my model

  public function get_question_by_testid($id) { 
    $this->db->select('question, description, name'); 
    $this->db->from('question'); 
    $this->db->join('test', 'test.id = question.testid'); 
  
    $this->db->where('testid', $id); 
    $query = $this->db->get(); 
    $result = $query->result_array(); 
    $count = count($result); 
  
    if (empty($count) || $count > 1) { 
      $question = null; return $question; 
    } else { 
      return $result;
    }
  }

why this code not work?

  //controller function test ($id = NULL) { 
    $data['tests'] = $this->student_model->get_test_by_id($id);
     $data['questions'] = $this->student_model->get_question_by_testid($id); 
    $this->load->view('studentExam',$data); 
  }

why does this code not work?

  //view foreach ($tests as $test) { 
    echo $test['name']; 
    echo '</br>'; echo $test['description'];
  } 
  foreach ($questions as $question) {
    echo $question['test']; 
    echo $question['question']; 
    echo '</br>';
  }
```

This question has several key issues. The user repeatedly asks, “why does this code not work” but does not provide any context, error messages, or specific expectations. Additionally, there is no indication that they have researched the issue prior to posting the question, nor is there evidence of any attempts to troubleshoot the issue on their own. This lack of detail and clarity makes it difficult for others to offer any meaningful assistance. Although this question did eventually receive an answer, questions of this nature are often overlooked or ignored, reflecting why clear and detailed questions are essential for effective problem solving.

## What Makes a ‘Smart’ Question?
In contrast, ‘smart’ questions possess the qualities that the ‘not so smart’ questions typically lack. They provide clear context, define the problem precisely, and show evidence of effort in solving it on their own.

Consider this next example. Although the title of the question, ‘_(Beginner Java issues) Why isn't this code working?_', is somewhat vague as well, we are provided with more clarity and detail. The way this user has formed their question allows others to better understand their problem and offer more effective solutions.
```
I have just handed in a lab for class where we had to make a class that describes a certain book. I could not figure out how to do two things. 1. If someone inputs a value less than zero for the 'pages' or 'suggestedRetailPrice' , the value must be set to zero. In this code the value is set 0 even if the value is positive. In the:

  if ( pages <= 0 ) { pages = 0; }

code if I set the second '0' to a different number, say:

  if ( pages <= 0 ) { pages = 1; }

Then the value for whatever you input for 'pages' will be 1. But shouldn't it be 1 ONLY if the value you input is a negative number? I don't get what I'm doing wrong.

The second thing I could not figure out is at the bottom of the code, we had to display all info. My teacher wanted us to display whether or not the book was paperback as 'yes' or 'no' instead of 'true' or 'false'. How do I do this? I tried putting an if/else statement in like this:
  System.out.println("Paperback : " + if (paperback = true) {Yes} if (paperback = false) {no}; )

Didn't work, can't figure it out. See whole code below.
…
```

The user provides a clear explanation of the issue, including a description of their expectations and previous attempts to fix the problem. This has made it significantly easier for others to understand the problem and offer useful assistance.

## Conclusion
Asking clear, well thought out questions is crucial in receiving helpful answers—not just on platforms like StackOverflow, but in any professional setting. By providing detailed context, outlining your expectations, and describing your own efforts to resolve the issue, you are more likely to receive a useful, equally detailed response. This not only helps you, but it also contributes positively to the community. On the other hand, poorly framed questions often go unanswered or ignored, representing missed opportunities for growth and learning. Whether you are a beginner or an expert, learning how to ask the right questions is an essential skill in software engineering and any field that involves daily problem solving.
