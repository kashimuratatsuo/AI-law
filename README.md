AI_LAW
-------------------------------------------------------------------------
all kinds of baseline models for long text classificaiton( text categorization)


Update: Joint Model for law cases prediction is released.

run python HAN_train.py to train the model for predict accusation, relevant articles and term of imprisonment.

challenges of this task:

   1) the description of law case(called facts) is quite long, the average words is around 400. it is not only long, but contain lots of information,

      even for a human being, you need to pay lots of attention before you can tell what's it about. for machine it need to have ability to handle long distance dependency,

      and pay attention on most important information.

   2) multiple sub tasks are included in this task. you are not only to predict accusations, but also need to predict relevant articles and term of imprisonment.

   3) this is a multi-label classification problem. given a fact, it may exists one or more than one accusations and serveral relevant articles.

   4) this also a imbalanced classification problem, while some labels have many data, other labels only have few data. to get best performance, you are not only

      to balanced precision and recall for a single label, but also need to balanced importance among different labels based on requirement or your evaluation matrix.




